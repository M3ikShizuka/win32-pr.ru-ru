---
description: Метод Сетдибдата указывает сведения о независимом от устройства GDI (DIB), который управляет этим объектом. Вызовите этот метод, чтобы инициализировать объект Цимажесампле.
ms.assetid: 850fa16b-d4b9-4fe6-b202-7b54c49a4589
title: Цимажесампле. Сетдибдата, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageSample.SetDIBData
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 418263da0416b325b1b080713dd6289f3bcc688e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127273067"
---
# <a name="cimagesamplesetdibdata-method"></a>Цимажесампле. Сетдибдата, метод

`SetDIBData`Метод указывает сведения о независимом от устройства GDI (DIB), который управляет этим объектом. Вызовите этот метод, чтобы инициализировать объект **Цимажесампле** .

## <a name="syntax"></a>Синтаксис


```C++
void SetDIBData(
   DIBDATA *pDibData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пдибдата* 
</dt> <dd>

Указатель на структуру [**дибдата**](dibdata.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Цимажесампле**](cimagesample.md)
</dt> </dl>

 

 




