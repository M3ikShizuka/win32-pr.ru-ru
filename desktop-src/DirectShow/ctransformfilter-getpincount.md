---
description: Метод Жетпинкаунт извлекает количество ПИН-кодов в фильтре.
ms.assetid: 29039ada-fccd-4890-b36b-3dd5c0bbdc3e
title: Ктрансформфилтер. Жетпинкаунт, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformFilter.GetPinCount
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ba1d2046bf7be31a9c0d3f3d43b13aeeffd1f76b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246676"
---
# <a name="ctransformfiltergetpincount-method"></a>Ктрансформфилтер. Жетпинкаунт, метод

`GetPinCount`Метод извлекает количество ПИН-кодов в фильтре.

## <a name="syntax"></a>Синтаксис


```C++
virtual int GetPinCount();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 2.

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**кбасефилтер:: жетпинкаунт**](cbasefilter-getpincount.md) . Класс **ктрансформфилтер** поддерживает ровно один входной ПИН-код и один выходной ПИН-код.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ктрансформфилтер**](ctransformfilter.md)
</dt> </dl>

 

 




