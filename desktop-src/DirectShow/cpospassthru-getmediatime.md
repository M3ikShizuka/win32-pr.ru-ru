---
description: Кпоспасссру. Жетмедиатиме, метод Жетмедиатиме извлекает метки времени для текущего образца.
ms.assetid: 36f3b6d3-b884-4168-94f3-f334a5056c7d
title: Кпоспасссру. Жетмедиатиме, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPosPassThru.GetMediaTime
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ec2767f3a20b6acc162da8670eefcd6d399639d5acf713b6dc54caf56f6edabe
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120084174"
---
# <a name="cpospassthrugetmediatime-method"></a>Кпоспасссру. Жетмедиатиме, метод

`GetMediaTime`Метод получает метки времени для текущего образца.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT GetMediaTime(
   LONGLONG *pStartTime,
   LONGLONG *pEndTime
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстарттиме* 
</dt> <dd>

Указатель на переменную, которая получает время начала в единицах текущего формата времени.

</dd> <dt>

*пендтиме* 
</dt> <dd>

Указатель на переменную, которая получает время окончания в единицах текущего формата времени.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение E \_ Fail.

## <a name="remarks"></a>Remarks

Переопределите этот метод, если фильтр кэширует метки времени на получаемых образцах.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кпоспасссру**](cpospassthru.md)
</dt> </dl>

 

 




