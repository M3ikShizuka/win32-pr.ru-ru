---
description: Возвращает число объектов Cursor, связанных с планшетом.
ms.assetid: 7aa5802c-1255-41a4-b1fa-23e5f56c0b80
title: 'Метод Итаблет:: Жеткурсоркаунт'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITablet.GetCursorCount
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: 2309384e4aa36383277ba72cc407cabef7ab4b27
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570378"
---
# <a name="itabletgetcursorcount-method"></a>Метод Итаблет:: Жеткурсоркаунт

Возвращает число объектов Cursor, связанных с планшетом.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetCursorCount(
  [out] ULONG *pcCurs
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пккурс* \[ заполняет\]
</dt> <dd>

Число объектов Cursor, связанных с планшетом.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Итаблет**](itablet.md)
</dt> </dl>

 

 




