---
description: Кдинамикаутпутпин. Деливербегинфлуш, метод Деливербегинфлуш запрашивает подключенный входной ПИН-код для начала операции очистки.
ms.assetid: eafc3835-7696-480b-abc8-154938e19b15
title: Кдинамикаутпутпин. Деливербегинфлуш, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDynamicOutputPin.DeliverBeginFlush
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 06b7486fa8fbacb4f2d048da198a78aa763e9beabc1991b2ddd178b9a55781b3
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120055944"
---
# <a name="cdynamicoutputpindeliverbeginflush-method"></a>Кдинамикаутпутпин. Деливербегинфлуш, метод

`DeliverBeginFlush`Метод запрашивает подключенный входной ПИН-код для начала операции очистки.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT DeliverBeginFlush();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК в случае успешного выполнения или **HRESULT** , указывающий на причину сбоя.

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**кбасеаутпутпин::D еливербегинфлуш**](cbaseoutputpin-deliverbeginflush.md) . Он устанавливает событие [**кдинамикаутпутпин:: m \_ хстопевент**](cdynamicoutputpin-m-hstopevent.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кдинамикаутпутпин**](cdynamicoutputpin.md)
</dt> </dl>

 

 




