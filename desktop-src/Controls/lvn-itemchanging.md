---
title: Код уведомления LVN_ITEMCHANGING (Коммктрл. h)
description: Сообщает родительскому окну элемента управления "представление списка", что элемент изменяется. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: ed6b5fc2-7e8c-4392-aa39-498b18922a98
keywords:
- LVN_ITEMCHANGING кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_ITEMCHANGING
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6183cd218792a34276db75dce5953189a8118674
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065770"
---
# <a name="lvn_itemchanging-notification-code"></a>\_Код уведомления ЛВН итемчангинг

Сообщает родительскому окну элемента управления "представление списка", что элемент изменяется. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_ITEMCHANGING

    pnmv = (LPNMLISTVIEW) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) , которая идентифицирует элемент и указывает, какие из его атрибутов изменяются.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , чтобы предотвратить изменение, или **false** , чтобы разрешить изменение.

## <a name="remarks"></a>Remarks

Если элемент управления "представление списка" имеет стиль [**LVS \_ ОВНЕРДАТА**](list-view-window-styles.md) , ЛВН \_ итемчангинг коды уведомлений не отправляются.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





