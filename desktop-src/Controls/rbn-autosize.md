---
title: Код уведомления RBN_AUTOSIZE (Коммктрл. h)
description: Посылается элементом управления главной панели, созданным с помощью стиля автомасштабирования RBS, \_ когда Главная панель автоматически изменяет размер. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: d174fe99-13cc-404c-9dc5-d5a93e9807a2
keywords:
- RBN_AUTOSIZE кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- RBN_AUTOSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 18ecfac5a4f84d69d444c25a24956cb911fd90a4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167239"
---
# <a name="rbn_autosize-notification-code"></a>\_Код уведомления РБН AUTOSIZE

Посылается элементом управления главной панели, созданным с помощью стиля автомасштабирования [**RBS \_**](rebar-control-styles.md) , когда Главная панель автоматически изменяет размер. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
RBN_AUTOSIZE

    lpnmas = (LPNMRBAUTOSIZE) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмрбаутосизе**](/windows/win32/api/commctrl/ns-commctrl-nmrbautosize) , содержащую сведения об операции изменения размера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого уведомления не используется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





