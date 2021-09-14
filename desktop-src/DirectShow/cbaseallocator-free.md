---
description: Метод Free освобождает всю буферную память. Этот метод вызывается, когда фильтр-владелец отменяет распределитель, после освобождения последнего примера носителя.
ms.assetid: dd1e6c4d-762a-4caf-902b-015c6c9fdb4d
title: Метод Кбасеаллокатор. Free (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.Free
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 3534eac01a6769e090c8c808f16cc6ad5c6b84c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347103"
---
# <a name="cbaseallocatorfree-method"></a>Кбасеаллокатор. Free, метод

`Free`Метод освобождает всю буферную память. Этот метод вызывается, когда фильтр-владелец отменяет распределитель, после освобождения последнего примера носителя.

## <a name="syntax"></a>Синтаксис


```C++
virtual void Free() = 0;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

После вызова метода [**uncommit**](cbaseallocator-decommit.md) распределитель вызывает этот метод при освобождении последнего примера носителя. Производный класс должен реализовывать этот метод.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




