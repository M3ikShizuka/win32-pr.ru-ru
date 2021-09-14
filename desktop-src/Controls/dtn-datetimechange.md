---
title: Код уведомления DTN_DATETIMECHANGE (Коммктрл. h)
description: Отправляется элементом управления "Выбор даты и времени" каждый раз, когда происходит изменение. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 65cdd8fb-1f07-4447-b503-d40fdfa37202
keywords:
- DTN_DATETIMECHANGE кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- DTN_DATETIMECHANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a40072a54732a0a3575e3153ddb901ca1df291b2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054777"
---
# <a name="dtn_datetimechange-notification-code"></a>\_Код уведомления ДТН датетимечанже

Отправляется элементом управления "Выбор даты и времени" каждый раз, когда происходит изменение. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
DTN_DATETIMECHANGE

    lpChange = (LPNMDATETIMECHANGE) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмдатетимечанже**](/windows/win32/api/commctrl/ns-commctrl-nmdatetimechange) , содержащую сведения об изменении, которое произошло в элементе управления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Владелец элемента управления должен возвращать ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





