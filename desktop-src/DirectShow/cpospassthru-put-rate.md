---
description: '\_Метод курса размещения задает скорость воспроизведения. Этот метод реализует метод Имедиапоситион::p UT \_ .'
ms.assetid: c077f344-de34-4f8a-8e08-6d7086a5a4f1
title: Метод CPosPassThru.put_Rate (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPosPassThru.put_Rate
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 21e7e654233f78adcda2addf73b87a178654872e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058019"
---
# <a name="cpospassthruput_rate-method"></a>Кпоспасссру. помещает \_ метод Rate

`put_Rate`Метод задает скорость воспроизведения. Этот метод реализует метод [**имедиапоситион::p UT \_**](/windows/desktop/api/Control/nf-control-imediaposition-put_rate) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_Rate(
   double dRate
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*драте* 
</dt> <dd>

Скорость воспроизведения. Не должно быть нулем.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает E \_ INVALIDARG, если *драте* равен нулю. В противном случае возвращает значение **HRESULT** из подключенного ПИН-кода.

## <a name="remarks"></a>Remarks

Отрицательные тарифы указывают на обратную игру. Не все носители будут поддерживать обратную воспроизведение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кпоспасссру**](cpospassthru.md)
</dt> </dl>

 

 




