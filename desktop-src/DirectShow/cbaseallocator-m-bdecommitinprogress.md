---
description: Флаг, указывающий, выполняется ли операция дефиксации.
ms.assetid: aa008be1-8faa-4dc1-9641-37dcc59ce6c7
title: 'Элемент Кбасеаллокатор:: m_bDecommitInProgress (Амфилтер. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_bDecommitInProgress
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 27aaf2766f67ebb77250522346cfe5c76acdf6d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058116"
---
# <a name="cbaseallocatorm_bdecommitinprogress-member"></a>Элемент Кбасеаллокатор:: m \_ бдекоммитинпрогресс

Флаг, указывающий, выполняется ли операция дефиксации. Значение равно **true** после вызова метода [**кбасеаллокатор::D екоммит**](cbaseallocator-decommit.md) , но до освобождения всех буферов. Если значение равно **true**, метод [**кбасеаллокатор::-buffer**](cbaseallocator-getbuffer.md) завершается ошибкой. Кроме того, распределитель не должен удалять себя, пока значение равно **true**.

## <a name="syntax"></a>Синтаксис


```C++
BOOL m_bDecommitInProgress;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




