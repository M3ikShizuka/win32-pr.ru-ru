---
description: Метод Сетваитинг увеличивает число ожидающих потоков.
ms.assetid: 4aec6177-fb32-44be-a58e-41a4f4aaf4f2
title: Кбасеаллокатор. Сетваитинг, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.SetWaiting
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 92cba22e128a76f7884050d74a7819142c696dc9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058091"
---
# <a name="cbaseallocatorsetwaiting-method"></a>Кбасеаллокатор. Сетваитинг, метод

`SetWaiting`Метод увеличивает число ожидающих потоков.

## <a name="syntax"></a>Синтаксис


```C++
void SetWaiting();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод увеличивает значение переменной члена [**кбасеаллокатор:: m \_ лваитинг**](cbaseallocator-m-lwaiting.md) . Если поток заблокирован в методе [**кбасеаллокатор::-buffer**](cbaseallocator-getbuffer.md) , распределитель вызывает метод `SetWaiting` , а затем ожидает сигнала для семафора [**\_ хсем кбасеаллокатор:: m**](cbaseallocator-m-hsem.md) . Метод [**кбасеаллокатор:: релеасебуффер**](cbaseallocator-releasebuffer.md) сигнализирует о семафоре и устанавливает для *m \_ лваитинг* обратно в нуль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




