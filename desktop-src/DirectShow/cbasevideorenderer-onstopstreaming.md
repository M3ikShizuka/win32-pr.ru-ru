---
description: Метод Онстопстреаминг вызывается в конце потоковой передачи, чтобы исправить время для отчета страницы свойств.
ms.assetid: 92174edb-2f6c-4bad-91c5-769aaebcc495
title: Кбасевидеорендерер. Онстопстреаминг, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.OnStopStreaming
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 08cf23fd2e1a7e854625d8a369d15290591386fe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173791"
---
# <a name="cbasevideorendereronstopstreaming-method"></a>Кбасевидеорендерер. Онстопстреаминг, метод

`OnStopStreaming`Метод вызывается в конце потоковой передачи, чтобы исправить время для отчета страницы свойств.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT OnStopStreaming();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Эта функция-член вызывается дважды, один раз при приостановке и снова, когда поток фактически останавливается.

Эта функция члена переопределяет [**кбасерендерер:: онстопстреаминг**](cbaserenderer-onstopstreaming.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




