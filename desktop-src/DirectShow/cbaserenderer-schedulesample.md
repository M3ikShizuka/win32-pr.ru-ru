---
description: Метод Счедулесампле планирует пример для подготовки к просмотру.
ms.assetid: 08c218d1-6d0a-4c66-bbde-a39e5d31561c
title: Кбасерендерер. Счедулесампле, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.ScheduleSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c340e54f35b353820b128681cfbc0c5798d38849
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254461"
---
# <a name="cbaserendererschedulesample-method"></a>Кбасерендерер. Счедулесампле, метод

`ScheduleSample`Метод планирует пример для отрисовки.

## <a name="syntax"></a>Синтаксис


```C++
virtual BOOL ScheduleSample(
   IMediaSample *pMediaSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмедиасампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) образца.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если образец был запланирован, или **значение false** , если образец был удален.

## <a name="remarks"></a>Remarks

Этот метод сначала определяет, должен ли образец быть визуализирован немедленно, визуализирован в будущем или удален. (Для этого вызывается метод [**кбасерендерер:: жетсамплетимес**](cbaserenderer-getsampletimes.md) .) Если образец должен быть визуализирован немедленно, метод сигнализирует о событии [**кбасерендерер:: m \_ рендеревент**](cbaserenderer-m-renderevent.md) . Если образец должен быть визуализирован в будущем, метод вызывает метод [**иреференцеклокк:: адвисетиме**](/windows/desktop/api/Strmif/nf-strmif-ireferenceclock-advisetime) для планирования.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




