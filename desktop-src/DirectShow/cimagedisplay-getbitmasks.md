---
description: Метод ВИДЕОИНФО извлекает цветовую маску для указанного формата.
ms.assetid: 72a9ba44-96de-4fff-a3fb-675d3dd080d8
title: Метод Цимажедисплай. с битовой маски (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageDisplay.GetBitMasks
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: dd8a3eac08a9e058f76e369a401429b69637f6438d60892d2632b88de0a0bb38
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120108464"
---
# <a name="cimagedisplaygetbitmasks-method"></a>Цимажедисплай..., метод

`GetBitMasks`Метод извлекает цветовую маску для указанного формата [**видеоинфо**](/previous-versions/windows/desktop/api/amvideo/ns-amvideo-videoinfo) .

## <a name="syntax"></a>Синтаксис


```C++
const DWORD* GetBitMasks(
   const VIDEOINFO *pVideoInfo
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пвидеоинфо* 
</dt> <dd>

Указатель на структуру **видеоинфо** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает массив из трех значений **типа DWORD** .

## <a name="remarks"></a>Remarks

Если элемент **бикомпрессион** является BI \_ битовых полей, метод возвращает указатель на цветовую маску, переданную в элементе **двбитмаскс** . Если элемент **бикомпрессион** является BI \_ RGB, метод возвращает цветовые маски, соответствующие глубине цвета. Если метод завершается ошибкой (например, глубина разрядности меньше 16), метод возвращает массив {0,0,0} .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Цимажедисплай**](cimagedisplay.md)
</dt> </dl>

 

 




