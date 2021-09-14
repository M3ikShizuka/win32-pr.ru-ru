---
description: Метод деструктора Кбасеаллокатор. ~ Кбасеаллокатор.
ms.assetid: b1e5653f-d72f-4cde-a8c9-d25763434374
title: Деструктор Кбасеаллокатор. ~ Кбасеаллокатор (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.~CBaseAllocator
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 9a4b754c8937b87a547f4583b3270f5782a6a415
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347111"
---
# <a name="cbaseallocatorcbaseallocator-destructor"></a>Деструктор Кбасеаллокатор. ~ Кбасеаллокатор

Метод деструктора.

## <a name="syntax"></a>Синтаксис


```C++
~CBaseAllocator();
```



## <a name="remarks"></a>Remarks

Всегда вызывайте метод [**кбасеаллокатор::D екоммит**](cbaseallocator-decommit.md) перед уничтожением объекта. Деструктор базового класса не может вызвать метод **uncommit**, так как этот метод вызывает чистый виртуальный метод [**Кбасеаллокатор:: Free**](cbaseallocator-free.md). Производные классы должны переопределять этот деструктор и вызывать метод **uncommit**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




