---
title: Сообщение CB_GETDROPPEDCONTROLRECT (Winuser. h)
description: Приложение отправляет \_ сообщение ЖЕТДРОППЕДКОНТРОЛРЕКТ CB для получения экранных координат поля со списком в состоянии его отклонения.
ms.assetid: fd8d78c0-e1a8-49c8-9e35-a105d00b863c
keywords:
- элементы управления Windows сообщений CB_GETDROPPEDCONTROLRECT
topic_type:
- apiref
api_name:
- CB_GETDROPPEDCONTROLRECT
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: adff5ad10ff91557b2579006dae6e1258650d74e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968737"
---
# <a name="cb_getdroppedcontrolrect-message"></a>\_Сообщение ЖЕТДРОППЕДКОНТРОЛРЕКТ CB

Приложение отправляет сообщение **\_ жетдроппедконтролрект CB** для получения экранных координат поля со списком в состоянии его отклонения.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**Rect**](/previous-versions//dd162897(v=vs.85)) , которая получает координаты поля со списком в его удаленном состоянии.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение прошло удачно, возвращаемое значение не равно нулю.

Если сообщение не выполняется, возвращаемое значение равно нулю.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ПЕРЕТАСКИВАЕМЫЕ**](/previous-versions//dd162897(v=vs.85))
</dt> </dl>

 

