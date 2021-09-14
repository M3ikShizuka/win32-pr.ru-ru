---
title: Сообщение HDM_GETFOCUSEDITEM (Коммктрл. h)
description: Возвращает элемент в элементе управления "заголовок", который находится в фокусе. Отправляйте это сообщение явным образом или с помощью \_ макроса Жетфокуседитем заголовка.
ms.assetid: 9ad8e497-6f81-4226-b138-d1101f2fd8b3
keywords:
- элементы управления Windows сообщений HDM_GETFOCUSEDITEM
topic_type:
- apiref
api_name:
- HDM_GETFOCUSEDITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6c21fcb29f5f431e32ca3f07265b7e96620d5a67
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054243"
---
# <a name="hdm_getfocuseditem-message"></a>\_Сообщение ЖЕТФОКУСЕДИТЕМ HDM

Возвращает элемент в элементе управления "заголовок", который находится в фокусе. Отправляйте это сообщение явным образом или с помощью макроса [**\_ жетфокуседитем заголовка**](/windows/desktop/api/Commctrl/nf-commctrl-header_getfocuseditem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Не используется. Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Не используется. Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс элемента в фокусе.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Сведения об элементах управления "заголовок"](header-controls.md)
</dt> </dl>

 

 





