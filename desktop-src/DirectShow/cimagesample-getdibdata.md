---
description: Метод Жетдибдата извлекает сведения о независимом от устройства GDI (DIB), который управляет этим объектом.
ms.assetid: ec337336-69ec-47ff-a522-42c0388f9bc0
title: Цимажесампле. Жетдибдата, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageSample.GetDIBData
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 0fd198152e7c0042a6d48cf942a48745540960d3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127273083"
---
# <a name="cimagesamplegetdibdata-method"></a>Цимажесампле. Жетдибдата, метод

`GetDIBData`Метод извлекает сведения о независимом от устройства GDI (DIB), который управляет этим объектом.

## <a name="syntax"></a>Синтаксис


```C++
DIBDATA* GetDIBData();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на структуру [**дибдата**](dibdata.md) .

## <a name="remarks"></a>Комментарии

Перед вызовом этого метода вызывающий объект должен инициализировать структуру **дибдата** ; Проверьте значение **Цимажесампле:: m \_ Бинит**. Чтобы инициализировать структуру, вызовите метод [**Цимажесампле:: сетдибдата**](cimagesample-setdibdata.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Цимажесампле**](cimagesample.md)
</dt> </dl>

 

 




