---
description: 'Метод Релеасебуффер возвращает пример носителя в список примеров бесплатных носителей. Этот метод реализует метод Имемаллокатор:: Релеасебуффер.'
ms.assetid: 35e4e426-044c-4e57-af13-2fddf8501db7
title: Кбасеаллокатор. Релеасебуффер, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.ReleaseBuffer
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 8e339f3a8186e845e28261633806a61b1b15c281
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058093"
---
# <a name="cbaseallocatorreleasebuffer-method"></a>Кбасеаллокатор. Релеасебуффер, метод

`ReleaseBuffer`Метод возвращает пример носителя в список примеров бесплатных носителей. Этот метод реализует метод [**имемаллокатор:: релеасебуффер**](/windows/desktop/api/Strmif/nf-strmif-imemallocator-releasebuffer) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ReleaseBuffer(
   IMediaSample *pSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) объекта Sample мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Remarks

Когда число ссылок в образце носителя достигает нуля, пример вызывает **релеасебуффер** в качестве параметра. Этот метод выполняет следующие действия.

-   Возвращает пример носителя в свободный список ([**кбасеаллокатор:: m \_ лфри**](cbaseallocator-m-lfree.md)).
-   Вызывает метод [**кбасеаллокатор:: нотифисампле**](cbaseallocator-notifysample.md) , который освобождает все потоки, заблокированные при вызове метода [**кбасеаллокатор::**](cbaseallocator-getbuffer.md) .
-   Если метод [**кбасеаллокатор:: сетнотифи**](cbaseallocator-setnotify.md) был вызван ранее, вызывается метод **Имемаллокаторнотификаллбакктемп:: нотифирелеасе** .
-   При освобождении последней выборки, если имеется ожидающий вызов [**кбасеаллокатор::D екоммит**](cbaseallocator-decommit.md) , вызывает метод [**Кбасеаллокатор:: Free**](cbaseallocator-free.md) для освобождения буферной памяти. (В базовом классе **Free** является чисто виртуальным методом.)

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




