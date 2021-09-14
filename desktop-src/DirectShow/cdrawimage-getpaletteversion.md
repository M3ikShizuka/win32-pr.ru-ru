---
description: Метод Жетпалеттеверсион извлекает текущую версию палитры.
ms.assetid: 9f97a810-04a4-4ea3-8918-416e9cd8e5e4
title: Кдравимаже. Жетпалеттеверсион, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDrawImage.GetPaletteVersion
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c86f1a0dad8d33913a52962dfe2ec09b7b8244db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053535"
---
# <a name="cdrawimagegetpaletteversion-method"></a>Кдравимаже. Жетпалеттеверсион, метод

`GetPaletteVersion`Метод получает текущую версию палитры.

## <a name="syntax"></a>Синтаксис


```C++
LONG GetPaletteVersion();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение переменной члена **m \_ палеттеверсион** .

## <a name="remarks"></a>Комментарии

Значение, возвращаемое этим методом, применяется только в том случае, если распределитель является объектом [**Цимажеаллокатор**](cimageallocator.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдравимаже**](cdrawimage.md)
</dt> <dt>

[**Кдравимаже:: Инкрементпалеттеверсион**](cdrawimage-incrementpaletteversion.md)
</dt> <dt>

[**Кдравимаже:: Ресетпалеттеверсион**](cdrawimage-resetpaletteversion.md)
</dt> </dl>

 

 




