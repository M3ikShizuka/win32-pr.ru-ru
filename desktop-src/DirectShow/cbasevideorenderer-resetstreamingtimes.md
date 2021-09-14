---
description: Метод Ресетстреамингтимес сбрасывает все значения времени, которые управляют потоковой передачей.
ms.assetid: 8a596760-a45a-4486-bb91-aab10bbf927f
title: Кбасевидеорендерер. Ресетстреамингтимес, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.ResetStreamingTimes
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: d887ca9e246d5e3fb746c119b1ed6784201ec702
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058060"
---
# <a name="cbasevideorendererresetstreamingtimes-method"></a>Кбасевидеорендерер. Ресетстреамингтимес, метод

`ResetStreamingTimes`Метод сбрасывает все значения времени, которые управляют потоковой передачей.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT ResetStreamingTimes();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Время задается таким образом, чтобы фреймы не удалялись изначально, а первый кадр был нарисован.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




