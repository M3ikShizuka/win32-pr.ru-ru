---
title: Код уведомления LVN_DELETEITEM (Коммктрл. h)
description: Сообщает родительскому окну элемента управления "представление списка", что элемент собирается удалиться. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 6e3d1955-ee35-488b-8b96-3d6ebbe5ceb5
keywords:
- LVN_DELETEITEM кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_DELETEITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 009d39e78aa93d5c5230e9c1b06b84d2854a0d0d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065780"
---
# <a name="lvn_deleteitem-notification-code"></a>\_Код уведомления ЛВН DELETEITEM

Сообщает родительскому окну элемента управления "представление списка", что элемент собирается удалиться. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_DELETEITEM

    pnmv = (LPNMLISTVIEW) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) . Член **Член iItem** определяет удаляемый элемент. Если у элемента управления нет стиля **LVS \_ овнердата** , то параметр *lParam* является определяемыми приложением данными, связанными с элементом. Все остальные члены этой структуры равны нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Не добавляйте, удаляйте и не Переупорядочивайте элементы в представлении списка при обработке этого кода уведомления.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





