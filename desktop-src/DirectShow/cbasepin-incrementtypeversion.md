---
description: Метод Инкременттипеверсион увеличивает номер версии в наборе предпочтительных типов носителей.
ms.assetid: 30cad0ae-58e7-47f6-94ee-75e24ce0a7e9
title: Кбасепин. Инкременттипеверсион, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePin.IncrementTypeVersion
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 6db3c08972bebbaf1172c44412ae9c8652100da8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971889"
---
# <a name="cbasepinincrementtypeversion-method"></a>Кбасепин. Инкременттипеверсион, метод

`IncrementTypeVersion`Метод увеличивает номер версии в наборе предпочтительных типов носителей.

## <a name="syntax"></a>Синтаксис


```C++
void IncrementTypeVersion();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Этот метод увеличивает значение переменной члена [**кбасепин:: m \_ типеверсион**](cbasepin-m-typeversion.md) . Если ПИН-код динамически изменяет список предпочтительных типов мультимедиа, вызывайте этот метод при каждом изменении списка. Дополнительные сведения см. в разделе [**кбасепин:: жетмедиатипеверсион**](cbasepin-getmediatypeversion.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




