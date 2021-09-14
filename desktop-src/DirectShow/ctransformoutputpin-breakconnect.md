---
description: Ктрансформаутпутпин. Бреакконнект, метод Бреакконнект освобождает ПИН-код из соединения.
ms.assetid: bf68aca3-93e5-4f9d-9980-1a5eed1513f5
title: Ктрансформаутпутпин. Бреакконнект, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformOutputPin.BreakConnect
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 92854041e1d553945d0a1ab1755ef3557bd4a8b2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255400"
---
# <a name="ctransformoutputpinbreakconnect-method"></a>Ктрансформаутпутпин. Бреакконнект, метод

`BreakConnect`Метод освобождает ПИН-код из соединения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT BreakConnect();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение, равное ОК или другому значению **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**кбасеаутпутпин:: бреакконнект**](cbaseoutputpin-breakconnect.md) . Он вызывает метод [**ктрансформфилтер:: бреакконнект**](ctransformfilter-breakconnect.md) фильтра, который возвращает \_ значение s ОК в базовом классе. Производный класс может переопределить метод **ктрансформфилтер:: бреакконнект** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




