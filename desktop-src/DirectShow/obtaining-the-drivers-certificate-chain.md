---
description: Получение цепочки сертификатов драйверов
ms.assetid: bc7b346c-3382-4f2b-90b6-03f6a1a5a9ce
title: Получение цепочки сертификатов драйверов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0c3f46e395550ca4bcb02396fe09126c1232f2c2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362388"
---
# <a name="obtaining-the-drivers-certificate-chain"></a>Получение цепочки сертификатов драйверов

чтобы использовать протокол сертифицированной защиты выхода (копп), приложение сначала должно создать диаграмму DirectShow, включающую фильтр рендеринга видео микширования (vmr-7 или VMR-9). Старый фильтр модуля подготовки отчетов не поддерживает Копп. Перед вызовом любых методов Копп приложение должно создать граф воспроизведения видео и подключить декодер к входному ПИН-коду фильтра VMR. Воспроизвести видеофайл необязательно.

После построения графа запросите VMR для интерфейса [**иамцертифиедаутпутпротектион**](/windows/desktop/api/Strmif/nn-strmif-iamcertifiedoutputprotection) , а затем вызовите [**Иамцертифиедаутпутпротектион:: кэйексчанже**](/windows/desktop/api/Strmif/nf-strmif-iamcertifiedoutputprotection-keyexchange). Этот метод возвращает 128-разрядное случайное число, введенное в виде GUID, а также указатель на массив байтов, содержащий цепочку сертификатов XML драйвера в формате UTF-8. В следующем коде показано, как получить цепочку сертификатов.


```C++
GUID guidRandom;
BYTE *pbCertificateChain = NULL;
DWORD cbCertificateChainLen;   // Size of the certificate chain, in bytes.
hr = pCOPP->KeyExchange(&guidRandom, &pbCertificateChain,
         &cbCertificateChainLen);
if (SUCCEEDED(hr))
{
    // TODO: Validate the certificate chain and get the driver's
    // public key. 

    // When you are done, free the buffer that contains the 
    // certificate chain.
    CoTaskMemFree(pbCertificateChain);
}
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование протокола сертифицированной выходной защиты (Копп)](using-certified-output-protection-protocol--copp.md)
</dt> </dl>

 

 



