---
description: 'Ксаурцесикинг. Сетрате, метод Сетрате задает скорость воспроизведения. Этот метод реализует метод Имедиасикинг:: Сетрате.'
ms.assetid: 954e2381-207a-47d9-a0a5-87dc325f52b4
title: Ксаурцесикинг. Сетрате, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.SetRate
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: f51b0425837cc48176490ea5d5d35cd2eae1851e7e56fa35b3578e37898afdd8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120053884"
---
# <a name="csourceseekingsetrate-method"></a>Ксаурцесикинг. Сетрате, метод

`SetRate`Метод задает скорость воспроизведения. Этот метод реализует метод [**имедиасикинг:: сетрате**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-setrate) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetRate(
   double dRate
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*драте* 
</dt> <dd>

Скорость воспроизведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод обновляет значение переменной члена [**ксаурцесикинг:: m \_ дратесикинг**](csourceseeking-m-drateseeking.md) , а затем вызывает чистый виртуальный метод [**ксаурцесикинг:: чанжерате**](csourceseeking-changerate.md). Метод не проверяет параметр *драте* .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




