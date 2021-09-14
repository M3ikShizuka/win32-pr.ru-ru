---
description: 'Метод Куеридиректион извлекает направление ПИН-кода (ввод или вывод). Этот метод реализует метод Ипин:: Куеридиректион.'
ms.assetid: c28332dc-5ac4-4c89-98b4-281424f36ba9
title: Кбасепин. Куеридиректион, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePin.QueryDirection
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 7e2ebfaa3d12b5f582b4b67014280fa0a0d5299d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254482"
---
# <a name="cbasepinquerydirection-method"></a>Кбасепин. Куеридиректион, метод

`QueryDirection`Метод получает направление ПИН-кода (ввод или вывод). Этот метод реализует метод [**Ипин:: куеридиректион**](/windows/desktop/api/Strmif/nf-strmif-ipin-querydirection) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT QueryDirection(
   PIN_DIRECTION *pPinDir
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппиндир* 
</dt> <dd>

Указатель на переменную, которая получает элемент перечисляемого [**типа \_ направления**](/windows/win32/api/strmif/ne-strmif-pin_direction) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ (ОК) или \_ указатель E.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




