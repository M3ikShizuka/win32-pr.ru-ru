---
description: Метод Словрендер рисует изображение видео с помощью функций Сетдибитстодевице или Стретчдибитс.
ms.assetid: e1d8b189-b588-48eb-988a-3e5dedb38dbd
title: Кдравимаже. Словрендер, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDrawImage.SlowRender
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b736bf6c44d4ada6e0a28408c449c9f8b2f1e1cb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053522"
---
# <a name="cdrawimageslowrender-method"></a>Кдравимаже. Словрендер, метод

`SlowRender`Метод рисует изображение видео с помощью функций **Сетдибитстодевице** или **стретчдибитс** .

## <a name="syntax"></a>Синтаксис


```C++
void SlowRender(
   IMediaSample *pMediaSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмедиасампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) образца, который содержит изображение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Если [**кдравимаже:: усингимажеаллокатор**](cdrawimage-usingimageallocator.md) возвращает **значение false**, то метод [**кдравимаже::D равимаже**](cdrawimage-drawimage.md) использует `SlowRender` для рисования видеоизображения. В противном случае DrawImage использует метод **фастрендер** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдравимаже**](cdrawimage.md)
</dt> <dt>

[**Кдравимаже:: Фастрендер**](cdrawimage-fastrender.md)
</dt> </dl>

 

 




