---
title: Код уведомления TVN_BEGINRDRAG (Коммктрл. h)
description: Сообщает родительскому окну элемента управления иерархического представления об инициации операции перетаскивания, включающей правую кнопку мыши. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 4a61d8b5-ceb9-46a3-95ef-27e843e8c986
keywords:
- TVN_BEGINRDRAG кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- TVN_BEGINRDRAG
- TVN_BEGINRDRAGA
- TVN_BEGINRDRAGW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bec15b5f48d4ed5612778622bb3655ae153c1b9f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165576"
---
# <a name="tvn_beginrdrag-notification-code"></a>\_Код уведомления ТВН бегинрдраг

Сообщает родительскому окну элемента управления иерархического представления об инициации операции перетаскивания, включающей правую кнопку мыши. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
TVN_BEGINRDRAG 

    pnmtv = (LPNMTREEVIEW) lParam 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмтривиев**](/windows/win32/api/commctrl/ns-commctrl-nmtreeviewa) . Элемент **итемнев** — это структура [**твитем**](/windows/win32/api/commctrl/ns-commctrl-tvitema) , которая содержит допустимые сведения в членах **хитем**, **State** и **lParam** о перемещенном элементе. Элемент **птдраг** указывает текущие экранные координаты мыши.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ТВН \_ БЕГИНРДРАГВ** (Юникод) и **ТВН \_ бегинрдрага** (ANSI)<br/>             |



 

 





