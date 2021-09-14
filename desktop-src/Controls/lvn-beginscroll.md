---
title: Код уведомления LVN_BEGINSCROLL (Коммктрл. h)
description: Сообщает родительскому окну элемента управления "представление списка", когда начинается операция прокрутки. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 67123db1-118c-43d7-8511-12a3c4413958
keywords:
- LVN_BEGINSCROLL кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- LVN_BEGINSCROLL
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ae09a05525ac6e9f08d8cc7a0b7de6ef51329baa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362613"
---
# <a name="lvn_beginscroll-notification-code"></a>\_Код уведомления ЛВН бегинскролл

Сообщает родительскому окну элемента управления "представление списка", когда начинается операция прокрутки. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
LVN_BEGINSCROLL

    pnmLVScroll = (LPNMLVSCROLL) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмлвскролл**](/windows/win32/api/commctrl/ns-commctrl-nmlvscroll) , содержащую горизонтальное или вертикальное расположение места начала операции прокрутки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не используется.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать этот код уведомления, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





