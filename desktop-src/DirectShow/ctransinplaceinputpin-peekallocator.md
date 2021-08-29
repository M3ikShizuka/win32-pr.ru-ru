---
description: Ктрансинплацеинпутпин. Пикаллокатор, метод Пикаллокатор возвращает указатель на распределитель контакта. Метод не увеличивает значение счетчика ссылок в интерфейсе.
ms.assetid: 67f1b872-4ae2-4fbe-9240-801ef8ae1e5b
title: Ктрансинплацеинпутпин. Пикаллокатор, метод (Трансип. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransInPlaceInputPin.PeekAllocator
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fbebca79b560ae2dfd10f95fc7b5f454228da017d6682b6f939ad504c624be72
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119999154"
---
# <a name="ctransinplaceinputpinpeekallocator-method"></a>Ктрансинплацеинпутпин. Пикаллокатор, метод

`PeekAllocator`Метод возвращает указатель на распределитель контакта. Метод не увеличивает значение счетчика ссылок в интерфейсе.

## <a name="syntax"></a>Синтаксис


```C++
IMemAllocator* PeekAllocator();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает переменную члена [**кбасеинпутпин:: m \_ паллокатор**](cbaseinputpin-m-pallocator.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансип. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ктрансинплацеинпутпин**](ctransinplaceinputpin.md)
</dt> </dl>

 

 




