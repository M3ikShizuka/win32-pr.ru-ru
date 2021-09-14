---
title: Код уведомления SBN_SIMPLEMODECHANGE (Коммктрл. h)
description: Посылается элементом управления "строка состояния" при изменении простого режима из-за \_ простого сообщения SB. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: b2df8feb-5028-4488-a99b-4ceff5b48a92
keywords:
- SBN_SIMPLEMODECHANGE кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- SBN_SIMPLEMODECHANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b998f0c39ecb00322bf5a423f99b3231338283f4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167056"
---
# <a name="sbn_simplemodechange-notification-code"></a>\_Код уведомления СБН симплемодечанже

Посылается элементом управления "строка состояния" при изменении простого режима из-за [**\_ простого сообщения SB**](sb-simple.md) . Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
SBN_SIMPLEMODECHANGE

    lpnmh = (NMHDR*) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr) , содержащую сведения о коде уведомления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется в строке состояния.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





