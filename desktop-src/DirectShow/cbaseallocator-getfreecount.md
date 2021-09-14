---
description: Метод Жетфрикаунт извлекает количество неиспользуемых выборок мультимедиа.
ms.assetid: f4ce4cca-0168-42db-9fe7-858862f033a8
title: Кбасеаллокатор. Жетфрикаунт, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.GetFreeCount
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a0538229053b5d47ca1bdc8f30b38a0937e36cb5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058127"
---
# <a name="cbaseallocatorgetfreecount-method"></a>Кбасеаллокатор. Жетфрикаунт, метод

`GetFreeCount`Метод получает количество неиспользуемых выборок мультимедиа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetFreeCount(
   LONG *plBuffersFree
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*плбуфферсфри* 
</dt> <dd>

Адрес переменной, которая получает количество неиспользуемых выборок.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Remarks

Этот метод реализует метод [**имемаллокаторкаллбакктемп:: жетфрикаунт**](/windows/desktop/api/Strmif/nf-strmif-imemallocatorcallbacktemp-getfreecount) . Распределитель не предоставляет интерфейс Имемаллокаторкаллбакктемп, если в конструкторе Кбасеаллокатор для флага *фенаблерелеасекаллбакк* не задано **значение true** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




