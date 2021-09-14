---
title: Сообщение STM_GETICON (Winuser. h)
description: Приложение отправляет \_ сообщение STM-Icon, чтобы получить маркер значка, связанного со статическим элементом управления, имеющим \_ стиль значка SS.
ms.assetid: e6b0a006-696b-401d-b894-b1db697c8939
keywords:
- элементы управления Windows сообщений STM_GETICON
topic_type:
- apiref
api_name:
- STM_GETICON
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f64f55d2a2f8315b99526e51a69891f6f0056e8b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167007"
---
# <a name="stm_geticon-message"></a>\_Сообщение STM

Приложение отправляет сообщение **STM- \_ Icon** , чтобы получить маркер значка, связанного со статическим элементом управления, имеющим \_ стиль значка SS.

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

Возвращаемое значение является обработчиком значка или **null** , если статический элемент управления не имеет связанного значка или если произошла ошибка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**STM \_ сетикон**](stm-seticon.md)
</dt> </dl>

 

 





