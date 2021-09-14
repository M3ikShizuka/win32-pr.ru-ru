---
title: Код уведомления LVN_COLUMNOVERFLOWCLICK (Коммктрл. h)
description: Отправляется элементом управления "представление списка" при нажатии кнопки переполнения. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 3d3bb7be-b598-450a-b829-a5aa5b1a0c5d
keywords:
- LVN_COLUMNOVERFLOWCLICK кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_COLUMNOVERFLOWCLICK
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7938d28be337f7255a9b84422fa090da5a494cc2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065782"
---
# <a name="lvn_columnoverflowclick-notification-code"></a>\_Код уведомления ЛВН колумноверфловкликк

Отправляется элементом управления "представление списка" при нажатии кнопки переполнения. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_COLUMNOVERFLOWCLICK
     
    pnmv = (LPNMLISTVIEW) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* \[ окне\]
</dt> <dd>

Указатель на структуру [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) , описывающую код уведомления. Вызывающий объект отвечает за выделение этой структуры, включая вложенную структуру [**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr) . Задайте элементы структуры **NMHDR** . Элемент **Code** должен иметь значение ЛВН \_ колумноверфловкликк.

Задайте для элемента **Член iItem** структуры [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) значение-1. Задайте для элемента **iSubItem** индекс подэлемента. Задайте для членов **уневстате**, **уолдстате** и **lParam** нулевое значение. Остальные элементы структуры **нмлиствиев** не используются.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Получатель уведомлений выполняет приведение *lParam* для получения структуры [**нмлиствиев**](/windows/win32/api/commctrl/ns-commctrl-nmlistview) . Параметр *wParam* содержит идентификатор элемента управления, который отправляет код уведомления.

Если элемент управления "заголовок" является дочерним элементом ListView, элемент управления "заголовок" должен отправить этот код уведомления в элемент управления ListView, когда элемент управления "заголовок" получает код уведомления [ХДН \_ оверфловкликк](hdn-overflowclick.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





