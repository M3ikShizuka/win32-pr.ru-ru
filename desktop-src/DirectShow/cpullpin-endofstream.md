---
description: Метод EndOfStream вызывается после того, как объект доставляет последнюю выборку. Производный класс должен реализовывать этот метод.
ms.assetid: 55a32c17-9993-4ad7-8829-6aa5c1407622
title: Кпуллпин. EndOfStream, метод (Пуллпин. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPullPin.EndOfStream
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a1df28430cdb71edd2ef9791e6c26092bbb21d0f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055560"
---
# <a name="cpullpinendofstream-method"></a>Кпуллпин. EndOfStream, метод

`EndOfStream`Метод вызывается после того, как объект доставляет последнюю выборку. Производный класс должен реализовывать этот метод.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT EndOfStream() = 0;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Этот метод используется для вызова [**Ипин:: EndOfStream**](/windows/desktop/api/Strmif/nf-strmif-ipin-endofstream) для каждого подчиненного входного контакта, получающего данные от этого объекта. Если закрепление вывода фильтра является производным от [**кбасеаутпутпин**](cbaseoutputpin.md), вызовите метод [**Кбасеаутпутпин::D еливерендофстреам**](cbaseoutputpin-deliverendofstream.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Пуллпин. h</dt> </dl>                                                                                                       |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Класс Кпуллпин**](cpullpin.md)
</dt> </dl>

 

 




