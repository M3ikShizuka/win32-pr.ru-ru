---
description: Метод Рекордфрамелатенесс записывает, как своевременно выполнялась визуализация, и собирает статистику для страницы свойств.
ms.assetid: 9d4b90d7-b529-40cc-a0fd-6635163fb7dd
title: Кбасевидеорендерер. Рекордфрамелатенесс, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.RecordFrameLateness
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 89682799ce71df8a8b08feb01454db3ec4fdd475a4107fcdb96e3a215a416657
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119814104"
---
# <a name="cbasevideorendererrecordframelateness-method"></a>Кбасевидеорендерер. Рекордфрамелатенесс, метод

`RecordFrameLateness`Метод записывает, как своевременно выполнялась визуализация, и собирает статистику для страницы свойств.

## <a name="syntax"></a>Синтаксис


```C++
virtual void RecordFrameLateness(
   int trLate,
   int trFrame
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*трлате* 
</dt> <dd>

Значение, указывающее, насколько поздно образец превысил время его выполнения в ссылочных единицах времени.

</dd> <dt>

*трфраме* 
</dt> <dd>

Время между кадрами, в ссылочных единицах времени.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




