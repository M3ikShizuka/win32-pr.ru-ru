---
title: Сообщение EM_GETMARGINS (Winuser. h)
description: Возвращает ширину левого и правого полей для элемента управления "поле ввода".
ms.assetid: 2482354b-aae0-4abd-8287-65c423f30abb
keywords:
- элементы управления Windows сообщений EM_GETMARGINS
topic_type:
- apiref
api_name:
- EM_GETMARGINS
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 239ad7e7888f5bceef60bf2719c3b67798b56220
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170075"
---
# <a name="em_getmargins-message"></a>\_Сообщение EM прибыли

Возвращает ширину левого и правого полей для элемента управления "поле ввода".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ширину левого поля в ЛОВОРД и ширину правого поля в HIWORD.

## <a name="remarks"></a>Remarks

**Расширенное редактирование:** Сообщение **EM \_ прибыли** не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EM \_ сетмаргинс**](em-setmargins.md)
</dt> </dl>

 

 





