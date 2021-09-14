---
title: Код уведомления LVN_DELETEALLITEMS (Коммктрл. h)
description: Сообщает родительскому окну элемента управления "представление списка", что все элементы в элементе управления будут удалены. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: e4a219cf-4af9-4d02-8810-f576ba658177
keywords:
- LVN_DELETEALLITEMS кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_DELETEALLITEMS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 583ad6e2372649ab5f63bd208fb97b93b1591c12
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362609"
---
# <a name="lvn_deleteallitems-notification-code"></a>\_Код уведомления ЛВН делетеаллитемс

Сообщает родительскому окну элемента управления "представление списка", что все элементы в элементе управления будут удалены. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_DELETEALLITEMS

    pnmv = (LPNMLISTVIEW) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) . Элемент **Член iItem** имеет значение-1, а остальные члены равны нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Чтобы отключить последующие коды уведомлений [ЛВН \_ DELETEITEM](lvn-deleteitem.md) , возвратите **значение true**.

Чтобы получить последующие коды уведомлений [ЛВН \_ DELETEITEM](lvn-deleteitem.md) , возвратите **значение false**.

## <a name="remarks"></a>Комментарии

Элемент управления "представление списка" отправляет код уведомления [**LVM \_ делетеаллитемс**](lvm-deleteallitems.md) при его уничтожении или при получении сообщения **LVM \_ делетеаллитемс** . Если **LVM \_ делетеаллитемс** не возвращает **значение true**, элемент управления также будет передавать код уведомления [ЛВН \_ DELETEITEM](lvn-deleteitem.md) по мере удаления каждого элемента.

Если обработчик сообщений [**LVM \_ делетеаллитемс**](lvm-deleteallitems.md) находится в процедуре диалогового окна, возвратите значение **true** из процедуры диалогового окна и используйте функцию [**SetWindowLong**](/windows/desktop/api/winuser/nf-winuser-setwindowlonga) с DWL мсгресулт, \_ чтобы установить возвращаемое значение сообщения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

