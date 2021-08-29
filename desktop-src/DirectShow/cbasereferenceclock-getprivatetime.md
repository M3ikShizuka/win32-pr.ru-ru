---
description: Метод Жетприватетиме извлекает значение реального времени из часов.
ms.assetid: ce9832cb-4b5a-49a1-9a69-d2fb90b3ed2e
title: Кбасереференцеклокк. Жетприватетиме, метод (Рефклокк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseReferenceClock.GetPrivateTime
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c8381f6e6e868fc6a57a65cf3bf124d90c035c854176265b2f9991356874e0ef
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120076504"
---
# <a name="cbasereferenceclockgetprivatetime-method"></a>Кбасереференцеклокк. Жетприватетиме, метод

`GetPrivateTime`Метод получает значение реального времени из часов.

## <a name="syntax"></a>Синтаксис


```C++
virtual REFERENCE_TIME GetPrivateTime();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает текущее время (в 100-наносекундных единицах).

## <a name="remarks"></a>Remarks

Этот метод возвращает реальное время, сообщаемое часами. Внешние вызывающие объекты используют метод [**кбасереференцеклокк:: OnTime**](cbasereferenceclock-gettime.md) , который вызывает этот метод. В отличие от метода со **временем** , внутренние часы могут проходить назад. Если это происходит, метод **метода noreturn по** ошибке возвращает время последнего отчета, пока метод не закончится `GetPrivateTime` .

Этот метод возвращает системное время. Переопределите этот метод, если часы получают время из другого источника.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>рефклокк. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасереференцеклокк**](cbasereferenceclock.md)
</dt> </dl>

 

 




