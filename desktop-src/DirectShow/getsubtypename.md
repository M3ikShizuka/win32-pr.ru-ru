---
description: Функция Жетсубтипенаме извлекает удобное для восприятия имя подтипа видео.
ms.assetid: 493b434e-2d36-4897-a5b2-7be0eb0a560f
title: Функция Жетсубтипенаме (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GetSubtypeName
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: f5cae835a3a7f1b5510d85ecf3f2ae9d15251a45
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053352"
---
# <a name="getsubtypename-function"></a>Функция Жетсубтипенаме

`GetSubtypeName`Функция получает удобное для восприятия имя подтипа видео.

## <a name="syntax"></a>Синтаксис


```C++
TCHAR* GetSubtypeName(
   const GUID *pSubtype
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псубтипе* 
</dt> <dd>

Указатель на **GUID** подтипа видео.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает строку, содержащую имя.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции видео и изображений](video-and-image-functions.md)
</dt> </dl>

 

 




