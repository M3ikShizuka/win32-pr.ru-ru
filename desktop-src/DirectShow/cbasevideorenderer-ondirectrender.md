---
description: Метод Ондиректрендер собирает сведения о времени, которые управляют синхронизацией и контролем качества.
ms.assetid: ed617fac-b2c6-4a3a-ac91-77e2d7cce981
title: Кбасевидеорендерер. Ондиректрендер, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.OnDirectRender
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: bb66169828d8649011c93f8daece4f0d389e82bef0f9d424cd59f2cdc9ae3cf6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120052174"
---
# <a name="cbasevideorendererondirectrender-method"></a>Кбасевидеорендерер. Ондиректрендер, метод

Метод **ондиректрендер** собирает сведения о времени, которые управляют синхронизацией и контролем качества.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT OnDirectRender(
   IMediaSample *pMediaSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмедиасампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) примера мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Вызовите этот метод вместо [**онрендерстарт**](cbasevideorenderer-onrenderstart.md) и [**онрендеренд**](cbasevideorenderer-onrenderend.md). Этот метод используется модулем подготовки видео DirectDraw.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




