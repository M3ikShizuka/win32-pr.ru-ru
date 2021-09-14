---
description: Кдинамикаутпутпин. Деливерендфлуш, метод Деливерендфлуш запрашивает подключенный входной ПИН-код для завершения операции очистки.
ms.assetid: e37bf06a-6cdc-4f14-bf2e-7a7d7004cff6
title: Кдинамикаутпутпин. Деливерендфлуш, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDynamicOutputPin.DeliverEndFlush
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c8b6952ff50dc2266655c58bd5c2e1ed13105598
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053986"
---
# <a name="cdynamicoutputpindeliverendflush-method"></a>Кдинамикаутпутпин. Деливерендфлуш, метод

`DeliverEndFlush`Метод запрашивает подключенный входной ПИН-код для завершения операции очистки.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT DeliverEndFlush();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК в случае успешного выполнения или **HRESULT** , указывающий на причину сбоя.

## <a name="remarks"></a>Комментарии

Этот метод переопределяет метод [**кбасеаутпутпин::D еливерендфлуш**](cbaseoutputpin-deliverendflush.md) . Он сбрасывает событие [**кдинамикаутпутпин:: m \_ хстопевент**](cdynamicoutputpin-m-hstopevent.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдинамикаутпутпин**](cdynamicoutputpin.md)
</dt> </dl>

 

 




