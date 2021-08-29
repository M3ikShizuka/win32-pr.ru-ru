---
description: Функция Валидатебитмапинфохеадер проверяет структуру БИТМАПИНФОХЕАДЕР для некоторых распространенных ошибок, которые могут привести к переполнению буфера или переполнению целочисленных значений.
ms.assetid: a797c286-ed77-437f-9ec1-1ef3a189bf62
title: Функция Валидатебитмапинфохеадер (Чеккбми. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ValidateBitmapInfoHeader
api_type:
- HeaderDef
api_location:
- checkbmi.h
ms.openlocfilehash: a23bbb322da1effdb2246ee797b353d1af36e3b87cbb37bd89039d1aced994e5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119755834"
---
# <a name="validatebitmapinfoheader-function"></a>Функция Валидатебитмапинфохеадер

`ValidateBitmapInfoHeader`Функция проверяет структуру [**битмапинфохеадер**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfoheader) для некоторых распространенных ошибок, которые могут привести к переполнению буфера или переполнению целочисленных значений.

> [!Note]  
> Эта функция не гарантирует, что структура [**битмапинфохеадер**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfoheader) является допустимой или что код, использующий структуру, является безопасным.

 

## <a name="syntax"></a>Синтаксис


```C++
BOOL ValidateBitmapInfoHeader(
   const BITMAPINFOHEADER *pbmi,
         DWORD            cbSize
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пбми* 
</dt> <dd>

Указатель на структуру [**битмапинфохеадер**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfoheader) для проверки.

</dd> <dt>

*кбсизе* 
</dt> <dd>

Размер блока памяти, в котором хранится структура, в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает логическое значение. Если значение равно **false**, структура [**битмапинфохеадер**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfoheader) недопустима.

## <a name="remarks"></a>Remarks

Эта функция защищает от следующих ошибок:

-   Арифметическое переполнение при размере структуры или недопустимом размере структуры.
-   Недопустимое значение для элемента **биклрусед** .
-   Арифметическое переполнение в размере изображения (**бисизеимаже**).
-   Недопустимые значения для размера изображения (**бисизеимаже**) для форматов RGB.

Функция не проверяет, описывает ли структура допустимый формат видео.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Чеккбми. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции видео и изображений](video-and-image-functions.md)
</dt> </dl>

 

 




