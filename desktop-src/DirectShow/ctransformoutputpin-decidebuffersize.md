---
description: Ктрансформаутпутпин. ДеЦидебуфферсизе, метод ДеЦидебуфферсизе задает требования к буферу.
ms.assetid: cdf9e384-623e-46a6-b123-d881fe21fb09
title: Ктрансформаутпутпин. ДеЦидебуфферсизе, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformOutputPin.DecideBufferSize
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1bc84eaf5e95a19436de5429ce018352cdaa286e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255367"
---
# <a name="ctransformoutputpindecidebuffersize-method"></a>Ктрансформаутпутпин. ДеЦидебуфферсизе, метод

`DecideBufferSize`Метод задает требования к буферу.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT DecideBufferSize(
   IMemAllocator        *pAlloc,
   ALLOCATOR_PROPERTIES *ppropInputRequest
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*паллок* 
</dt> <dd>

Указатель на интерфейс [**имемаллокатор**](/windows/desktop/api/Strmif/nn-strmif-imemallocator) распределителя.

</dd> <dt>

*ппропинпутрекуест* 
</dt> <dd>

Указатель на [**структуру \_ свойств распределителя**](/windows/win32/api/strmif/ns-strmif-allocator_properties) , которая содержит требования к буферу входного контакта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Этот метод переопределяет метод [**кбасеаутпутпин::D еЦидебуфферсизе**](cbaseoutputpin-decidebuffersize.md) . Он вызывает чисто виртуальный метод [**ктрансформфилтер::D еЦидебуфферсизе**](ctransformfilter-decidebuffersize.md) для фильтра, который должен реализовываться производным классом фильтра.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




