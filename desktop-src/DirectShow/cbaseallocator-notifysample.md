---
description: Метод Нотифисампле освобождает все потоки, ожидающие выборки.
ms.assetid: b09c48a0-9cd5-44a7-9267-d2a11e8cde4c
title: Кбасеаллокатор. Нотифисампле, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.NotifySample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: acaf5e45eac6a630d0589e3c8fad106ae29fa3dc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058094"
---
# <a name="cbaseallocatornotifysample-method"></a>Кбасеаллокатор. Нотифисампле, метод

`NotifySample`Метод освобождает все потоки, ожидающие выборки.

## <a name="syntax"></a>Синтаксис


```C++
void NotifySample();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Если имеются потоки, ожидающие выборки, значение [**кбасеаллокатор:: m \_ лваитинг**](cbaseallocator-m-lwaiting.md) больше нуля. Если значение *m \_ лваитинг* больше нуля, этот метод вызывает функцию **ReleaseSemaphore** для семафора [**кбасеаллокатор:: m \_ хсем**](cbaseallocator-m-hsem.md) , активируя все ожидающие потоки. Он также сбрасывает значение *m \_ лваитинг* до нуля.

Этот метод вызывается из метода [**кбасеаллокатор:: релеасебуффер**](cbaseallocator-releasebuffer.md) , когда образец возвращается в свободный список. и из метода [**кбасеаллокатор::D екоммит**](cbaseallocator-decommit.md) , когда распределитель является незафиксированным.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




