---
description: Метод Сетпопевент указывает событие, сообщающее, когда объект удаляет образец из очереди.
ms.assetid: 147a09b9-14d3-4739-843a-1bfb19d2d052
title: Каутпуткуеуе. Сетпопевент, метод (Аутпутк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- COutputQueue.SetPopEvent
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e499d756d983cbd5849f3178bc3ed26d0d4194bd15e1e220462f86d2f3e9a00e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119909444"
---
# <a name="coutputqueuesetpopevent-method"></a>Каутпуткуеуе. Сетпопевент, метод

`SetPopEvent`Метод указывает событие, сообщающее, когда объект удаляет выборку из очереди.

## <a name="syntax"></a>Синтаксис


```C++
void SetPopEvent(
   HANDLE hEvent
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хевент* 
</dt> <dd>

Обработчик события, созданного вызывающим объектом.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




