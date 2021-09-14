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
ms.openlocfilehash: f7a5f7cb0fbe754890b1d7930bb54c6fca47afa5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971569"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансип. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ктрансинплацеинпутпин**](ctransinplaceinputpin.md)
</dt> </dl>

 

 




