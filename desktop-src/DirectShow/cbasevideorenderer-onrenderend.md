---
description: Метод Онрендеренд выполняет сглаживание для случаев, когда время отрисовки меняется из-за прерываний.
ms.assetid: 561b3306-0c41-4f04-b73a-78e7b4038e86
title: Кбасевидеорендерер. Онрендеренд, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.OnRenderEnd
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 8f37b4d03f77090f4cac40a218fd3ac27c0c349d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173811"
---
# <a name="cbasevideorendereronrenderend-method"></a>Кбасевидеорендерер. Онрендеренд, метод

`OnRenderEnd`Метод выполняет сглаживание для случаев, когда время отрисовки меняется из-за прерываний.

## <a name="syntax"></a>Синтаксис


```C++
void OnRenderEnd(
   IMediaSample *pMediaSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмедиасампле* 
</dt> <dd>

Указатель на пример носителя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Эту функцию члена следует вызывать сразу после рисования изображения.

Эта функция члена переопределяет [**кбасерендерер:: онрендеренд**](cbaserenderer-onrenderend.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




