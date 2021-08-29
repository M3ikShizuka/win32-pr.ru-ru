---
description: 'Метод Жетсинксаурце извлекает ссылочное время, которое использует фильтр. Этот метод реализует метод Имедиафилтер:: Жетсинксаурце.'
ms.assetid: b8c95838-bd6e-41c5-b3ab-71ebb33136f0
title: Кбасефилтер. Жетсинксаурце, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseFilter.GetSyncSource
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 632350f925f843f05bdf7820bc8c14a4570f152afc741d5ed58f1827ad205251
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120056554"
---
# <a name="cbasefiltergetsyncsource-method"></a>Кбасефилтер. Жетсинксаурце, метод

`GetSyncSource`Метод получает ссылочное время, которое использует фильтр. Этот метод реализует метод [**имедиафилтер:: жетсинксаурце**](/windows/desktop/api/Strmif/nf-strmif-imediafilter-getsyncsource) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetSyncSource(
   IReferenceClock **pClock
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пклокк* 
</dt> <dd>

Адрес переменной, которая получает указатель на интерфейс [**иреференцеклокк**](/windows/desktop/api/Strmif/nn-strmif-ireferenceclock) часов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ (ОК) или \_ указатель E.

## <a name="remarks"></a>Remarks

Если в фильтре не используется ссылочное время, *\* пклокк* имеет значение **null**. Если метод возвращает значение, если *\* пклокк* не равен **null**, то интерфейс **иреференцеклокк** имеет необработанный счетчик ссылок. Не забудьте освободить его по завершении.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасефилтер**](cbasefilter.md)
</dt> </dl>

 

 




