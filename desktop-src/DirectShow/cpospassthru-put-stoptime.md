---
description: Метод размещения \_ StopTime задает время, когда воспроизведение будет прервано относительно длительности потока. Этот метод реализует метод Имедиапоситион::p UT \_ StopTime.
ms.assetid: 0a344cad-df93-47f1-8c7f-5d5ef775b850
title: Метод CPosPassThru.put_StopTime (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPosPassThru.put_StopTime
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4f5763700947596a0fb437ba3840df058d4d3239
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058018"
---
# <a name="cpospassthruput_stoptime-method"></a>Кпоспасссру. размещение \_ метода StopTime

`put_StopTime`Метод задает время, когда воспроизведение будет останавливаться, относительно длительности потока. Этот метод реализует метод [**имедиапоситион::p UT \_ StopTime**](/windows/desktop/api/Control/nf-control-imediaposition-put_stoptime) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_StopTime(
   REFTIME llTime
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ллтиме* 
</dt> <dd>

Время окончания в секундах. 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** из подключенного ПИН-кода.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кпоспасссру**](cpospassthru.md)
</dt> </dl>

 

 




