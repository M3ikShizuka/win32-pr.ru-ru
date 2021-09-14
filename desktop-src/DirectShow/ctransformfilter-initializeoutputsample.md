---
description: Метод Инитиализеаутпутсампле извлекает новый образец вывода и инициализирует его.
ms.assetid: a4f8f514-cf1a-4f8f-ac17-17378705c2ea
title: Ктрансформфилтер. Инитиализеаутпутсампле, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformFilter.InitializeOutputSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: efe7e62936c6feb1984a339a67783cdbc1e4f124
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246679"
---
# <a name="ctransformfilterinitializeoutputsample-method"></a>Ктрансформфилтер. Инитиализеаутпутсампле, метод

`InitializeOutputSample`Метод получает новый выходной пример и инициализирует его.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT InitializeOutputSample(
   IMediaSample *pSample,
   IMediaSample **ppOutSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) образца входных данных.

</dd> <dt>

*ппаутсампле* 
</dt> <dd>

Получает указатель на интерфейс **имедиасампле** образца выходных данных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение, равное ОК или другому значению **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод вызывается методом [**ктрансформфилтер:: Receive**](ctransformfilter-receive.md) для подготовки выходного примера. Как правило, нет необходимости вызывать этот метод в производном классе, если не переопределить метод **Receive** .

Этот метод получает новый пример из распределителя выходного контакта. Затем он копирует примеры свойств из примера входных данных в образец Output. Примеры свойств определяются в структуре [**\_ \_ свойств SAMPLE2**](/windows/win32/api/strmif/ns-strmif-am_sample2_properties) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ктрансформфилтер**](ctransformfilter.md)
</dt> </dl>

 

 




