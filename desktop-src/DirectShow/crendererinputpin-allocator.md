---
description: Метод распределителя извлекает указатель на распределитель памяти.
ms.assetid: ac262502-eadc-482c-bc58-1e942889f0a7
title: Метод Крендереринпутпин. распределитель (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CRendererInputPin.Allocator
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 9bf30b9d2aaad9f879baf5b0122589150ebff814a73f2f3c85c2ca72c6886308
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119908474"
---
# <a name="crendererinputpinallocator-method"></a>Крендереринпутпин. распределитель, метод

`Allocator`Метод получает указатель на распределитель памяти.

## <a name="syntax"></a>Синтаксис


```C++
IMemAllocator* Allocator() const;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на интерфейс [**имемаллокатор**](/windows/desktop/api/Strmif/nn-strmif-imemallocator) распределителя или **значение NULL**.

## <a name="remarks"></a>Remarks

Этот метод возвращает переменную члена [**кбасеинпутпин:: m \_ паллокатор**](cbaseinputpin-m-pallocator.md) . Метод не увеличивает значение счетчика ссылок в интерфейсе. Этот метод является исключительно методом доступа.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Крендереринпутпин**](crendererinputpin.md)
</dt> </dl>

 

 




