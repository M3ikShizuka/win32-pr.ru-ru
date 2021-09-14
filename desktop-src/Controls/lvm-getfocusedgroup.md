---
title: Сообщение LVM_GETFOCUSEDGROUP (Коммктрл. h)
description: Возвращает группу, в которой находится фокус. Отправьте это сообщение явным образом или с помощью \_ макроса Жетфокуседграуп ListView.
ms.assetid: c1902f35-84b7-4f46-89a6-e48148f06172
keywords:
- элементы управления Windows сообщений LVM_GETFOCUSEDGROUP
topic_type:
- apiref
api_name:
- LVM_GETFOCUSEDGROUP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3e0d12eb637ec1a421a5eaff58636df7bef8f449
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054100"
---
# <a name="lvm_getfocusedgroup-message"></a>\_Сообщение LVM жетфокуседграуп

Возвращает группу, в которой находится фокус. Отправьте это сообщение явным образом или с помощью макроса [**\_ жетфокуседграуп ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_getfocusedgroup) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс группы с состоянием ЛВГС \_ Focused или-1, если нет группы с состоянием лвгс \_ Focused.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





