---
description: Метод Ready сигнализирует о завершении перехода состояния.
ms.assetid: 01328281-cf25-43fd-9f9c-e55fccbac217
title: Метод Кбасерендерер. ready (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.Ready
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 3a7f70ec258fde7f6208d44c35ca2c284f99e0a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058071"
---
# <a name="cbaserendererready-method"></a>Кбасерендерер. ready, метод

`Ready`Метод сигнализирует о завершении перехода состояния.

## <a name="syntax"></a>Синтаксис


```C++
void Ready();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод приводит к тому, что метод [**кбасерендерер::**](cbaserenderer-getstate.md) noreturn возвращает значение S \_ OK, что означает, что фильтр завершил переход в текущее состояние. Фильтр вызывает этот метод при каждом завершении смены состояния.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> <dt>

[**Кбасерендерер:: Чеккреади**](cbaserenderer-checkready.md)
</dt> <dt>

[**Кбасерендерер:: NotReady**](cbaserenderer-notready.md)
</dt> </dl>

 

 




