---
description: Метод Stopped определяет, остановлен ли фильтр, содержащий этот ПИН-код.
ms.assetid: ffeac352-2f9b-44be-a8e8-7e9238d0b18e
title: Метод Кбасепин. Stopped (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePin.IsStopped
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4185c02b396f7d0d570081ba1401e0ec9e301d46
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971882"
---
# <a name="cbasepinisstopped-method"></a>Кбасепин. метод Stopped

`IsStopped`Метод определяет, остановлен ли фильтр, содержащий этот ПИН-код.

## <a name="syntax"></a>Синтаксис


```C++
BOOL IsStopped();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если фильтр остановлен. В противном случае возвращает **значение false**.

## <a name="remarks"></a>Комментарии

Не вызывайте этот метод из в методе конструктора **кбасепин** , так как фильтр, возможно, еще не инициализирован.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




