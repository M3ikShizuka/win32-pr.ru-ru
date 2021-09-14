---
description: Блокировка для защиты создания объектов внутри фильтра.
ms.assetid: ad1d2584-0d9e-42a8-83ea-0c1907ddcf33
title: 'Элемент Кбасерендерер:: m_ObjectCreationLock (Ренбасе. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_ObjectCreationLock
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e344b20b4924ac26ebe6253f5388136b350abefe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058077"
---
# <a name="cbaserendererm_objectcreationlock-member"></a>Элемент Кбасерендерер:: m \_ обжекткреатионлокк

Блокировка для защиты создания объектов внутри фильтра. Фильтр удерживает эту блокировку при создании входного ПИН-кода ([**кбасерендерер:: m \_ пинпутпин**](cbaserenderer-m-pinputpin.md)) или объекта [**крендерерпоспасссру**](crendererpospassthru.md) ([**кбасерендерер:: m \_ ппоситион**](cbaserenderer-m-pposition.md)). Эта блокировка предотвращает одновременную попытку создания одного из этих объектов несколькими потоками.

## <a name="syntax"></a>Синтаксис


```C++
CCritSec m_ObjectCreationLock;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




