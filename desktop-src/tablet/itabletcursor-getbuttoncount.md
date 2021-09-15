---
description: Получает количество кнопок пера планшета.
ms.assetid: ae4ce670-769a-4f00-b728-285020f09934
title: 'Метод Итаблеткурсор:: Жетбуттонкаунт'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITabletCursor.GetButtonCount
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: 08fdf24b2a0b69b7830a683786f18fc5df0805b2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574471"
---
# <a name="itabletcursorgetbuttoncount-method"></a>Метод Итаблеткурсор:: Жетбуттонкаунт

Получает количество кнопок пера планшета.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetButtonCount(
  [out] ULONG *pcButtons
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пкбуттонс* \[ заполняет\]
</dt> <dd>

Число кнопок пера планшета.

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

[**Интерфейс Итаблеткурсор**](itabletcursor.md)
</dt> </dl>

 

 




