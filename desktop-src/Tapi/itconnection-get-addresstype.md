---
description: Метод Get \_ addressType получает тип адреса.
ms.assetid: b2ff6303-6beb-429c-ad1a-2f729749e5db
title: 'Метод Итконнектион:: get_AddressType (Сдпблб. h)'
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d015b0b395f0219fa9a7af2ca7002f242cfaa1b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064571"
---
# <a name="itconnectionget_addresstype-method"></a>Метод Итконнектион:: Get \_ addressType

\[встречи и элементы управления встречными IP-телефонными соединениями недоступны для использования в Windows Vista, Windows Server 2008 и последующих версиях операционной системы. API клиента RTC предоставляет аналогичные функциональные возможности.\]

Метод **Get \_ addressType** получает тип адреса.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_AddressType(
  [out] BSTR *ppAddressType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппаддресстипе* \[ заполняет\]
</dt> <dd>

Указатель на **строку BSTR** , содержащую тип адреса.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                                   | Описание                                                      |
|-----------------------------------------------------------------------------------------------|------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Метод успешно выполнен.<br/>                                     |
| <dl> <dt>**\_указатель E**</dt> </dl>     | Параметр *ппаддресстипе* не является допустимым указателем.<br/> |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl> | Недостаточно памяти для выполнения операции.<br/>  |
| <dl> <dt>**\_Ошибка E**</dt> </dl>        | Незаданная ошибка.<br/>                                    |
| <dl> <dt>**E \_ нотимпл**</dt> </dl>     | Этот метод еще не реализован.<br/>                   |



 

## <a name="remarks"></a>Remarks

Приложение должно использовать [**сисфристринг**](/windows/win32/api/oleauto/nf-oleauto-sysfreestring) для освобождения памяти, выделенной для параметра *ппаддресстипе* .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------|---------------------------------------------------------------------------------------|
| Версия TAPI<br/> | Требуется TAPI 3,0 или более поздней версии<br/>                                                 |
| Заголовок<br/>       | <dl> <dt>Сдпблб. h</dt> </dl>   |
| Библиотека<br/>      | <dl> <dt>UUID. lib</dt> </dl>   |
| DLL<br/>          | <dl> <dt>Sdpblb.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**итконнектион**](itconnection.md)
</dt> <dt>

[**Итконнектион::p \_ addressType**](itconnection-put-addresstype.md)
</dt> </dl>

 

