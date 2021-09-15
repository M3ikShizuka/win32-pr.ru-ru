---
description: Помещает элемент в очередь.
ms.assetid: 8ac41d80-e7d5-4b3f-9f09-c3d39c94c490
title: Ккуеуе. Путкуеуеобжект, метод (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CQueue.PutQueueObject
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 5371c843bb348f50539535a3df9a0f6aed00893e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461947"
---
# <a name="cqueueputqueueobject-method"></a>Ккуеуе. Путкуеуеобжект, метод

Помещает элемент в очередь.

## <a name="syntax"></a>Синтаксис


```C++
void PutQueueObject(
   T object
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*object* 
</dt> <dd>

Объект типа **T** (тип шаблона).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод блокируется до тех пор, пока в очереди элемента не будет свободного пространства.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ккуеуе**](cqueue.md)
</dt> </dl>

 

 




