---
title: Код уведомления LVN_ODSTATECHANGED (Коммктрл. h)
description: Отправляется элементом управления "представление списка" при изменении состояния элемента или диапазона элементов. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: a3aafda5-a3ec-4f84-8153-8d34097e04f1
keywords:
- LVN_ODSTATECHANGED кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_ODSTATECHANGED
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bdf8712078e3398f775115233c0fd54622943cc2cb7febe0c24d800776418de5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915114"
---
# <a name="lvn_odstatechanged-notification-code"></a>\_Код уведомления ЛВН одстатечанжед

Отправляется элементом управления "представление списка" при изменении состояния элемента или диапазона элементов. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_ODSTATECHANGED

    lpStateChange = (LPNMLVODSTATECHANGE) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмлводстатечанже**](/windows/win32/api/commctrl/ns-commctrl-nmlvodstatechange) , которая содержит сведения об измененном элементе или элементах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Приложение, получающее этот код уведомления, должно возвращать ноль.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





