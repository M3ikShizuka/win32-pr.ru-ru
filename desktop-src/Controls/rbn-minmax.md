---
title: Код уведомления RBN_MINMAX (Коммктрл. h)
description: Посылается элементом управления "Главная панель" до максимизации или минимизации полосы. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 75619cb0-ef0b-44fa-83b2-15a5e5e92c60
keywords:
- RBN_MINMAX кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- RBN_MINMAX
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d18fea875af376b3ec9b311d2aad09597f0ce6ea264963e9e466cc87ce4fe4b6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119984994"
---
# <a name="rbn_minmax-notification-code"></a>\_Код уведомления РБН MINMAX

Посылается элементом управления "Главная панель" до максимизации или минимизации полосы. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
RBN_MINMAX
```



## <a name="parameters"></a>Параметры

Этот код уведомления не содержит параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение, чтобы не допустить выполнения операции, ноль, чтобы разрешить продолжение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





