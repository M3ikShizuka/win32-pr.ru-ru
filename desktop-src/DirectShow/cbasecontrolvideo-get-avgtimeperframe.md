---
description: Метод Get \_ авгтимеперфраме извлекает среднее время для каждого кадра.
ms.assetid: bcfdb241-9ec1-49f4-b2b5-0869c27da953
title: Метод CBaseControlVideo.get_AvgTimePerFrame (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlVideo.get_AvgTimePerFrame
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ae69140348be6e2fdfc120ee7fb40096d663f720
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347102"
---
# <a name="cbasecontrolvideoget_avgtimeperframe-method"></a>Кбасеконтролвидео. Get \_ авгтимеперфраме, метод

`get_AvgTimePerFrame`Метод получает среднее время для каждого кадра.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_AvgTimePerFrame(
   REFTIME *pAvgTimePerFrame
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*павгтимеперфраме* 
</dt> <dd>

Указатель на среднее время на кадр.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ошибку с ошибками в случае успеха или E \_ OUTOFMEMORY, если объем доступной памяти недостаточен.

## <a name="remarks"></a>Remarks

Эта функция члена реализует метод [**ибасиквидео:: Get \_ авгтимеперфраме**](/windows/desktop/api/Control/nf-control-ibasicvideo-get_avgtimeperframe) . Он вызывает чисто виртуальную функцию члена [**кбасеконтролвидео:: жетвидеоформат**](cbasecontrolvideo-getvideoformat.md) для получения структуры [**видеоинфохеадер**](/previous-versions/windows/desktop/api/amvideo/ns-amvideo-videoinfoheader) из производного класса.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвидео**](cbasecontrolvideo.md)
</dt> </dl>

 

 




