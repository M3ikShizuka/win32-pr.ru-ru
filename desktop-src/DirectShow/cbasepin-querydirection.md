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
ms.openlocfilehash: 3769b7cd510b21d91a0b855fa0551cf698b91812e5aab3fc53bda32bb4ce82cb
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120056234"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




