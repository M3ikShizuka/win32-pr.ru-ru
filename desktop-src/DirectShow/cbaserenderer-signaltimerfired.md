---
description: Метод Сигналтимерфиред очищает идентификатор таймера, используемый для планирования подготовки к просмотру.
ms.assetid: b8ae362e-fcda-4888-be32-8fb910d0f0db
title: Кбасерендерер. Сигналтимерфиред, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.SignalTimerFired
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4dd29b37869fc6f07c2d876dfa0d1d306b04b111
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054009"
---
# <a name="cbaserenderersignaltimerfired-method"></a>Кбасерендерер. Сигналтимерфиред, метод

`SignalTimerFired`Метод очищает идентификатор таймера, используемый для планирования подготовки к просмотру.

## <a name="syntax"></a>Синтаксис


```C++
virtual void SignalTimerFired();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Фильтр вызывает этот метод, когда таймер отрисовки активирует (см [**. кбасерендерер:: ваитфоррендертиме**](cbaserenderer-waitforrendertime.md)) или при отмене таймера (см. [**Кбасерендерер:: канцелнотификатион**](cbaserenderer-cancelnotification.md)). Метод сбрасывает переменную члена [**кбасерендерер:: m \_ двадвисе**](cbaserenderer-m-dwadvise.md) в нулевое значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




