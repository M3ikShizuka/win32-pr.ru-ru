---
description: Флаг, указывающий, отправил ли фильтр уведомление об окончании потока.
ms.assetid: 93f897de-04bb-4de4-a612-39b27c7d6f6c
title: 'Элемент Ктрансформфилтер:: m_bEOSDelivered (Трансфрм. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_bEOSDelivered
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: f24b87f9808c53b5f64f66031a8ee2a4e9449089
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246673"
---
# <a name="ctransformfilterm_beosdelivered-member"></a>Элемент Ктрансформфилтер:: m \_ беосделиверед

Флаг, указывающий, отправил ли фильтр уведомление об окончании потока.

## <a name="syntax"></a>Синтаксис


```C++
BOOL m_bEOSDelivered;
```



## <a name="remarks"></a>Remarks

Если фильтр приостанавливается, когда у него нет входного соединения, то он отправляет уведомление о завершении потока и устанавливает для этого флага **значение true**. Уведомление о завершении потока гарантирует, что нисходящий фильтр не ждет выборки. Обратите внимание, что метод [**EndOfStream**](ctransformfilter-endofstream.md) фильтра не устанавливает этот флаг.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ктрансформфилтер**](ctransformfilter.md)
</dt> </dl>

 

 




