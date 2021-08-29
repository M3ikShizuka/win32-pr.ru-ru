---
description: 'Метод Стартстреаминг вызывается, когда фильтр переключается в состояние паузы. Этот метод переопределяет метод Ктрансформфилтер:: Стартстреаминг.'
ms.assetid: fa05f88f-fed8-479d-b0b4-d9df982d51e7
title: Квидеотрансформфилтер. Стартстреаминг, метод (Втранс. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CVideoTransformFilter.StartStreaming
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 53d448228a650718f8c57d6019dcfb1f3f23f03468e86a77fae167e6481e718c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119998474"
---
# <a name="cvideotransformfilterstartstreaming-method"></a>Квидеотрансформфилтер. Стартстреаминг, метод

`StartStreaming`Метод вызывается, когда фильтр переключается в состояние паузы. Этот метод переопределяет метод [**ктрансформфилтер:: стартстреаминг**](ctransformfilter-startstreaming.md) .

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT StartStreaming();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Remarks

Этот метод сбрасывает всю статистику производительности.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>втранс. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Квидеотрансформфилтер**](cvideotransformfilter.md)
</dt> </dl>

 

 




