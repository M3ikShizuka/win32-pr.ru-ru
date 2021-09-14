---
description: Метод GetNext извлекает дескриптор события, который используется для сигнализации об изменении в следующем времени.
ms.assetid: 2548a321-df65-4a5b-9e6a-8bbc031254c7
title: Камсчедуле. четный (Дссчедуле. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAMSchedule.GetEvent
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 360a4b88c8c03d2f04ad55bc65eebf6be3797c92
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145229"
---
# <a name="camschedulegetevent-method"></a>Камсчедуле. четный, метод

`GetEvent`Метод получает дескриптор события, который используется для сигнализации об изменении в следующем времени.

## <a name="syntax"></a>Синтаксис


```C++
HANDLE GetEvent();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер события.

## <a name="remarks"></a>Remarks

Если следующее время уведомления изменилось другими словами, при добавлении нового запроса advise в начало списка планировщик сигнализирует об этом событии. Для определения следующего времени вызова в часах необходимо вызвать метод [**камсчедуле:: Advise**](camschedule-advise.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>дссчедуле. h (включает Потоки. h)</dt> </dl>                                                                                |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камсчедуле**](camschedule.md)
</dt> </dl>

 

 




