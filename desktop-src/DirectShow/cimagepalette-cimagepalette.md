---
description: Метод конструктора Цимажепалетте. Цимажепалетте.
ms.assetid: 50fa573c-a244-4a1e-9fd9-2b33a3427c84
title: Конструктор Цимажепалетте. Цимажепалетте (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImagePalette.CImagePalette
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 5021b165a8fa47bedc7961657d7cdbfa07af301d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055588"
---
# <a name="cimagepalettecimagepalette-constructor"></a>Цимажепалетте. Цимажепалетте, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CImagePalette(
   CBaseFilter *pBaseFilter,
   CBaseWindow *pBaseWindow,
   CDrawImage  *pDrawImage
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пбасефилтер* 
</dt> <dd>

Указатель на фильтр-владелец.

</dd> <dt>

*пбасевиндов* 
</dt> <dd>

Указатель на объект **кбасевиндов** , который управляет окном, в котором реализована палитра. Этот параметр может принимать значение **NULL**.

</dd> <dt>

*пдравимаже* 
</dt> <dd>

Указатель на объект **кдравимаже** , который рисует изображение видео. Этот параметр может принимать значение **NULL**.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Класс Цимажепалетте**](cimagepalette.md)
</dt> </dl>

 

 




