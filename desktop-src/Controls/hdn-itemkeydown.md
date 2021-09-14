---
title: Код уведомления HDN_ITEMKEYDOWN (Коммктрл. h)
description: Сообщает родительскому окну элемента управления заголовка, что нажата клавиша с выбранным элементом. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: ab6922ab-907d-44fc-8606-28f395118405
keywords:
- HDN_ITEMKEYDOWN кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- HDN_ITEMKEYDOWN
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4c4415eb5a026bf96d53884fe2735f3a3fa2e494
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054184"
---
# <a name="hdn_itemkeydown-notification-code"></a>\_Код уведомления ХДН итемкэйдовн

Сообщает родительскому окну элемента управления заголовка, что нажата клавиша с выбранным элементом. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
HDN_ITEMKEYDOWN

   pNMHeader = (LPNMHEADER) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмхеадер**](/windows/win32/api/commctrl/ns-commctrl-nmheadera) , которая содержит дополнительные сведения о нажатом ключе.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





