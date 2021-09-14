---
title: Код уведомления TBN_DRAGOVER (Коммктрл. h)
description: Определяет, \_ следует ли отправлять маркбуттон-ТБ сообщение для кнопки, для которой выполняется перетаскивание. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 2bb5c52e-0c90-4662-8ffd-045ecc7ed7e5
keywords:
- TBN_DRAGOVER кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- TBN_DRAGOVER
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cfa02aa8fabf89ea27fce628d3d63165255bbd66
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166376"
---
# <a name="tbn_dragover-notification-code"></a>\_Код уведомления ТБН DRAGOVER

Определяет, следует ли [**отправлять \_ Маркбуттон-ТБ**](tb-markbutton.md) сообщение для кнопки, для которой выполняется перетаскивание. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
TBN_DRAGOVER

    lpnmtb = (NMTBHOTITEM*) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмтбхотитем**](/windows/win32/api/commctrl/ns-commctrl-nmtbhotitem) , указывающую, к какому элементу выполняется перетаскивание.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

**Значение false** , если панель инструментов должна отправить \_ сообщение маркбуттон ТБ; в противном случае — **значение true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





