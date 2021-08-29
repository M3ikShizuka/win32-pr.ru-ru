---
description: Метод Жеттаржетрект извлекает прямоугольник назначения. Это внутренняя вспомогательная функция-член.
ms.assetid: bf9d95c9-eee8-46b8-bdee-a7d16777ed83
title: Кбасеконтролвидео. Жеттаржетрект, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlVideo.GetTargetRect
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 3309f36ed731ce0221e98a2a9f9b1459b31864a789a52d950951b613c23fdfbd
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119928794"
---
# <a name="cbasecontrolvideogettargetrect-method"></a>Кбасеконтролвидео. Жеттаржетрект, метод

`GetTargetRect`Метод извлекает прямоугольник назначения. Это внутренняя вспомогательная функция-член.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT GetTargetRect(
   RECT *pTargetRect
) = 0;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*птаржетрект* 
</dt> <dd>

Указатель на прямоугольник назначения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Эта функция члена должна быть переопределена в производном классе для возврата целевого прямоугольника, удерживаемого модулем подготовки видео. Он вызывается из следующих функций-членов [**кбасеконтролвидео**](cbasecontrolvideo.md) .

-   [**Кбасеконтролвидео:: Жетдестинатионпоситион**](cbasecontrolvideo-getdestinationposition.md)
-   [**Кбасеконтролвидео::p UT \_ дестинатионлефт**](cbasecontrolvideo-put-destinationleft.md)
-   [**Кбасеконтролвидео:: Get \_ дестинатионлефт**](cbasecontrolvideo-get-destinationleft.md)
-   [**Кбасеконтролвидео::p UT \_ дестинатионвидс**](cbasecontrolvideo-put-destinationwidth.md)
-   [**Кбасеконтролвидео:: Get \_ дестинатионвидс**](cbasecontrolvideo-get-destinationwidth.md)
-   [**Кбасеконтролвидео::p UT \_ дестинатионтоп**](cbasecontrolvideo-put-destinationtop.md)
-   [**Кбасеконтролвидео:: Get \_ дестинатионтоп**](cbasecontrolvideo-get-destinationtop.md)
-   [**Кбасеконтролвидео::p UT \_ дестинатионхеигхт**](cbasecontrolvideo-put-destinationheight.md)
-   [**Кбасеконтролвидео:: Get \_ дестинатионхеигхт**](cbasecontrolvideo-get-destinationheight.md)

В следующем примере демонстрируется реализация этой функции в производном классе.


```C++
// Return the current destination rectangle.
HRESULT CVideoText::GetTargetRect(RECT *pTargetRect)
{
    ASSERT(pTargetRect);
    m_pRenderer->m_DrawImage.GetTargetRect(pTargetRect);
    return NOERROR;
}
```



В этом примере Квидеотекст является классом, производным от [**кбасеконтролвидео**](cbasecontrolvideo.md), m \_ прендерер содержит объект класса, производного от [**кбасевидеорендерер**](cbasevideorenderer.md), и \_ член данных m DrawImage, определенный в производном классе, содержит объект [**кдравимаже**](cdrawimage.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвидео**](cbasecontrolvideo.md)
</dt> </dl>

 

 




