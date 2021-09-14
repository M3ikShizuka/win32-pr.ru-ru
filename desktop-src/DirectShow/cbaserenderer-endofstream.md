---
description: Метод EndOfStream уведомляет фильтр о том, что входной ПИН-код получил уведомление о завершении потока.
ms.assetid: bdfd03f9-81e0-4d52-959e-82fd1a67e1c3
title: Кбасерендерер. EndOfStream, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.EndOfStream
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 6e12da02ffbce99b29d324c1166b3d4cdf2265c6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053586"
---
# <a name="cbaserendererendofstream-method"></a>Кбасерендерер. EndOfStream, метод

`EndOfStream`Метод уведомляет фильтр о том, что входной ПИН-код получил уведомление об окончании потока.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT EndOfStream();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Комментарии

Входной ПИН-код фильтра вызывает этот метод при получении уведомления о завершении потока.

Этот метод задает для флага [**кбасерендерер:: m \_ Беос**](cbaserenderer-m-beos.md) **значение true** и вызывает метод [**кбасерендерер:: сендендофстреам**](cbaserenderer-sendendofstream.md) , чтобы запланировать событие [**\_ завершения EC**](ec-complete.md) . Если фильтр приостановлен и ожидает выборка, этот метод завершает переход состояния.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




