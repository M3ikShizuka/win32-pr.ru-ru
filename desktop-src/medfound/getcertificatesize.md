---
description: Возвращает размер сертификата для драйвера экрана.
ms.assetid: fd52e939-127a-4493-8406-31f7767921cd
title: Функция Жетцертификатесизе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GetCertificateSize
api_type:
- DllExport
api_location:
- gdi32.dll
ms.openlocfilehash: bcd1f49ce65978c6a89c89cee1fda38e41434065
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257920"
---
# <a name="getcertificatesize-function"></a>Функция Жетцертификатесизе

> [!IMPORTANT]
> Эта функция используется [выходными данными диспетчера защиты](output-protection-manager.md) (ОПМ) для доступа к функциям видеодрайвера. Приложения не должны вызывать эту функцию.

 

Возвращает размер сертификата для драйвера экрана.

## <a name="syntax"></a>Синтаксис


```C++
NTSTATUS WINAPI GetCertificateSize(
  _In_  PUNICODE_STRING          pstrDeviceName,
  _In_  DXGKMDT_CERTIFICATE_TYPE ctPVPCertificateType,
  _Out_ ULONG                    *pulCertificateLength
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстрдевиценаме* \[ окне\]
</dt> <dd>

Указатель на [**\_ строковую структуру Юникода**](/windows/win32/api/subauth/ns-subauth-unicode_string) , содержащую имя устройства вывода, которое возвращается функцией [**жетмониторинфо**](/windows/win32/api/winuser/nf-winuser-getmonitorinfoa) .

</dd> <dt>

*ктпвпцертификатетипе* \[ окне\]
</dt> <dd>

Тип сертификата, указанный как член перечисления **\_ \_ типа сертификата дксгкмдт** .

</dd> <dt>

*пулцертификателенгс* \[ заполняет\]
</dt> <dd>

Получает размер сертификата в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается успешно, возвращается **состояние \_ Success**. В противном случае возвращается код ошибки **NTSTATUS** .

## <a name="remarks"></a>Комментарии

Приложения должны вызывать метод [**иопмвидеуутпут:: стартинитиализатион**](/windows/desktop/api/opmapi/nf-opmapi-iopmvideooutput-startinitialization) вместо этой функции.

Эта функция не имеет связанной библиотеки импорта. Для вызова этой функции необходимо использовать функции [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) и [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) для динамической привязки к Gdi32.dll.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                 |
| DLL<br/>                      | <dl> <dt>Gdi32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции ОПМ](opm-functions.md)
</dt> <dt>

[Диспетчер выходной защиты](output-protection-manager.md)
</dt> </dl>

 

 
