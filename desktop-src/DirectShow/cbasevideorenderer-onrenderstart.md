---
description: Метод Онрендерстарт задает сведения для подготовки к просмотру.
ms.assetid: 698fe778-e2cb-4b87-a668-084b6c12c71f
title: Кбасевидеорендерер. Онрендерстарт, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.OnRenderStart
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 7327d25aafa6f6673b7ed70b658f675a9dab8f4d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173804"
---
# <a name="cbasevideorendereronrenderstart-method"></a>Кбасевидеорендерер. Онрендерстарт, метод

`OnRenderStart`Метод задает сведения для подготовки к просмотру.

## <a name="syntax"></a>Синтаксис


```C++
void OnRenderStart(
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

Эта функция-член получает текущее время часов из системы и сохраняет ее в переменной-члене, используемой при завершении рисования. Функция также выполняет ведение журнала производительности. Эту функцию члена следует вызывать непосредственно перед началом рисования.

Эта функция члена переопределяет [**кбасерендерер:: онрендерстарт**](cbaserenderer-onrenderstart.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




