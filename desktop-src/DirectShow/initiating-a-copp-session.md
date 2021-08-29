---
description: Запуск сеанса Копп
ms.assetid: c84a83b4-51b2-4b46-860f-d740b42323fa
title: Запуск сеанса Копп
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 72e3d952e7e938eee3eef27663ea075b3a5b23d4e61ef9f9fd0ea9b5395708cf
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119748674"
---
# <a name="initiating-a-copp-session"></a>Запуск сеанса Копп

Чтобы инициировать сеанс протокола Копп, необходимо подготовить *сигнатуру*, которая представляет собой массив, содержащий объединение следующих чисел:

-   128-разрядное случайное число, возвращенное драйвером. (Это значение отображается как *гуидрандом* при [получении цепочки сертификатов драйвера](obtaining-the-drivers-certificate-chain.md).)
-   128-битный симметричный ключ AES.
-   32-разрядный начальный порядковый номер для запросов состояния.
-   32-разрядный начальный порядковый номер для команд Копп.

Создайте симметричный ключ AES следующим образом:


```C++
DWORD dwFlag = 0x80;         // Bit length: 128-bit AES.
dwFlag <<= 16;               // Move this value to the upper 16 bits.
dwFlag |= CRYPT_EXPORTABLE;  // We want to export the key.
CryptGenKey(
    hCSP,           // Handle to the CSP.
    CALG_AES_128,   // Use 128-bit AES block encryption algorithm.
    dwFlag,
    &m_hAESKey      // Receives a handle to the AES key.
);
```



Функция **криптженкэй** создает симметричный ключ, но ключ по-прежнему ХРАНИТСЯ в CSP. Чтобы экспортировать ключ в массив байтов, используйте функцию **криптекспорткэй** . Это причина использования \_ флага для экспорта при вызове **криптженкэй**. Следующий код экспортирует ключ и копирует его в


```
pData
```



Массив.


```C++
DWORD cbData = 0; 
BYTE *pData = NULL;
// Get the size of the blob.
CryptExportKey(hAESKey, 0, PLAINTEXTKEYBLOB, 0, NULL, &cbData);  

// Allocate the array and call again.
pData = new BYTE[cbData];
CryptExportKey(hAESKey, 0, PLAINTEXTKEYBLOB, 0, pData, &cbData);  
```



Данные, возвращаемые в


```
pData
```



имеет следующий макет:


```C++
BLOBHEADER header
DWORD      cbSize
BYTE       key[]
```



Однако структура, соответствующая этому макету, не определена в заголовках CryptoAPI. Можно определить одну или несколько арифметических операций с указателями. Например, чтобы проверить размер ключа, выполните следующие действия.


```C++
DWORD *pcbKey = (DWORD*)(pData + sizeof(BLOBHEADER));
if (*pcbKey != 16)
{
    // Wrong size! Should be 16 bytes (128 bits).
}
```



Чтобы получить указатель на сам ключ, сделайте следующее:


```C++
BYTE *pKey = pData + sizeof(BLOBHEADER) + sizeof(DWORD);
```



Затем создайте 32-разрядное случайное число, которое будет использоваться в качестве начальной последовательности для запросов состояния Копп. Рекомендуемый способ создания случайного числа — вызов функции **CryptGenRandom** . Не используйте функцию **Rand** в библиотеке времени выполнения C, так как она не является действительно случайной. Создайте второе 32-разрядное случайное число, которое будет использоваться в качестве начальной последовательности команд Копп.


```C++
UINT uStatusSeq;     // Status sequence number.
UINT uCommandSeq;    // Command sequence number.
CryptGenRandom(hCSP, sizeof(UINT), &uStatusSeq);
CryptGenRandom(hCSP, sizeof(UINT), &uCommandSeq);
```



Теперь можно подготовить подпись Копп. Это 256-байтовый массив, определенный как структура [**амкоппсигнатуре**](/windows/win32/api/strmif/ns-strmif-amcoppsignature) . Инициализирует содержимое массива до нуля. Затем скопируйте четыре числа в массив — случайное число драйвера, ключ AES, порядковый номер состояния и порядковый номер команды в указанном порядке. Наконец, замените порядок байтов для всего массива.

В соответствии с документацией по **криптенкрипт**:

<dl> «Длина данных в виде открытого текста, которую можно зашифровать с помощью вызова **криптенкрипт** с помощью ключа RSA, — это длина модуля ключа минус 11 байт. 11 байт — это выбранный минимум для заполнения PKCS \# 1.  
</dl>

В этом случае значение модуля составляет 256 байт, поэтому максимальная длина сообщения — 245 байт (256 – 11). Структура **амкоппсигнатуре** составляет 256 байт, но значимые данные в сигнатуре — только 40 байт. Следующий код шифрует подпись и предоставляет результат в


```
CoppSig
```



.


```C++
AMCOPPSignature CoppSig;
ZeroMemory(&CoppSig, sizeof(CoppSig));
// Copy the signature data into CoppSig. (Not shown.)

// Encrypt the signature:
const DWORD RSA_PADDING = 11;    // 11-byte padding.
DWORD cbDataOut = sizeof(AMCOPPSignature);
DWORD cbDataIn = cbDataOut - RSA_PADDING;
CryptEncrypt(
    hRSAKey, 
    NULL,     // No hash object.
    TRUE,     // Final block to encrypt.
    0,        // Reserved.
    &CoppSig, // COPP signature.
    &cbDataOut, 
    cbDataIn
);
```



Теперь передайте зашифрованный массив в [**иамцертифиедаутпутпротектион:: сессионсекуенцестарт**](/windows/desktop/api/Strmif/nf-strmif-iamcertifiedoutputprotection-sessionsequencestart):


```C++
hr = pCOPP->SessionSequenceStart(&CoppSig);
if (SUCCEEDED(hr))
{
    // Ready to send COPP commands and status requests.
}
```



Если этот метод завершился удачно, вы можете отправить драйверу команды Копп и запросы о состоянии.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование протокола сертифицированной выходной защиты (Копп)](using-certified-output-protection-protocol--copp.md)
</dt> </dl>

 

 



