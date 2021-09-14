---
description: Метод размещения \_ CurrentPosition задает текущую точку относительно общей продолжительности потока. Этот метод реализует метод Имедиапоситион::p UT \_ CurrentPosition.
ms.assetid: 22d7e9e4-47da-45b5-9be0-3c5128f90353
title: Метод CPosPassThru.put_CurrentPosition (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPosPassThru.put_CurrentPosition
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 85426636a34d0e197b36496d5a38a847c61b9501
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058022"
---
# <a name="cpospassthruput_currentposition-method"></a>Кпоспасссру. размещение \_ метода CurrentPosition

`put_CurrentPosition`Метод задает текущую точку относительно общей продолжительности потока. Этот метод реализует метод [**имедиапоситион::p UT \_ CurrentPosition**](/windows/desktop/api/Control/nf-control-imediaposition-put_currentposition) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_CurrentPosition(
   REFTIME llTime
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ллтиме* 
</dt> <dd>

Новое расположение в секундах.

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

 

 




