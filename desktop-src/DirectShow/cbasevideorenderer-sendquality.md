---
description: Метод Сендкуалити отправляет сообщение с качеством, чтобы указать, что должен делать поставщик в отношении качества.
ms.assetid: 9ce11c35-958c-4eda-9130-1139c4074bf7
title: Кбасевидеорендерер. Сендкуалити, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.SendQuality
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 8a6ae7228be0f3012c49d652d11bf2c1c3bfc181
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055599"
---
# <a name="cbasevideorenderersendquality-method"></a>Кбасевидеорендерер. Сендкуалити, метод

`SendQuality`Метод отправляет сообщение с качеством, чтобы указать, что должен сделать поставщик о качестве качества.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT SendQuality(
   REFERENCE_TIME trLate,
   REFERENCE_TIME trRealStream
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*трлате* 
</dt> <dd>

Время, в течение которого кадр находится в конце.

</dd> <dt>

*трреалстреам* 
</dt> <dd>

Время куррентстреам.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Эта функция-член отправляет поток сообщений контроля качества в Управление качеством. Характер качественного сообщения (то есть необходимость уменьшить или увеличить количество выборок) определяется в реализации управления качеством в этом производном классе (см. [**кбасевидеорендерер:: шаулддравсампленов**](cbasevideorenderer-shoulddrawsamplenow.md)).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




