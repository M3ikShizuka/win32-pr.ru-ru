---
description: Преобразует URL-адрес файла в путь Microsoft MS-DOS.
ms.assetid: c35988ad-6cf8-41ec-bee9-e3bb982310ee
title: Функция Мфкреатепасфромурл
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- MFCreatePathFromURL
api_type:
- DllExport
api_location:
- mfplat.dll
ms.openlocfilehash: 5f4a2156bde837ef343aa4ca88a18230050d4af6df07012e46fc518d62d898af
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120113684"
---
# <a name="mfcreatepathfromurl-function"></a>Функция Мфкреатепасфромурл

\[Этот API не поддерживается и может быть изменен или недоступен в будущем. Вместо этого приложения должны вызывать [**паскреатефромурл**](/windows/win32/api/shlwapi/nf-shlwapi-pathcreatefromurla).\]

Преобразует URL-адрес файла в путь Microsoft MS-DOS.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT MFCreatePathFromURL(
  _In_opt_ LPCWSTR pwszFileURL,
  _Out_    LPWSTR  *ppwszFilePath
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пвсзфилеурл* \[ в необязательное\]
</dt> <dd>

Строка, завершающаяся нулем и содержащая URL-адрес. Максимальная длина строки — **\_ Максимальная \_ \_ Длина URL-адреса в Интернете**.

</dd> <dt>

*ппвсзфилепас* \[ заполняет\]
</dt> <dd>

Получает строку, завершающуюся нулем, которая содержит URL-адрес. Вызывающий объект должен освободить строку, вызвав [**CoTaskMemFree**](/windows/win32/api/combaseapi/nf-combaseapi-cotaskmemfree).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Функция возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                                  | Описание                                                                                                 |
|----------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Функция выполнена успешно. <br/>                                                                         |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимый аргумент. Строка, указанная в параметре *пвсзфилеурл* , не может быть преобразована в путь.<br/> |



 

## <a name="remarks"></a>Remarks

Эта функция не имеет связанной библиотеки импорта. Для вызова этой функции необходимо использовать функции [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) и [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) для динамической привязки к Mfplat.dll.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Mfplat.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции Media Foundation](media-foundation-functions.md)
</dt> </dl>

 

 
