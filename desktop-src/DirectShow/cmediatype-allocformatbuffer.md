---
description: Метод Аллокформатбуффер выделяет память для блока Format.
ms.assetid: 5ff716c7-f9cf-4b1c-9d3a-62ab955c1392
title: Кмедиатипе. Аллокформатбуффер, метод (Мтипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaType.AllocFormatBuffer
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: d6a9314fd06734adcc367b7be34dc8d6d1b9d996
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246850"
---
# <a name="cmediatypeallocformatbuffer-method"></a>Кмедиатипе. Аллокформатбуффер, метод

`AllocFormatBuffer`Метод выделяет память для блока Format.

## <a name="syntax"></a>Синтаксис


```C++
BYTE* AllocFormatBuffer(
   ULONG length
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*length* 
</dt> <dd>

Требуемый размер блока формата в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на новый блок в случае успеха. В противном случае возвращает **значение NULL**.

## <a name="remarks"></a>Remarks

Если метод успешно выделяет новый блок формата, он освобождает существующий блок формата. Если выделение завершается неудачей, метод оставляет существующий блок формата.

Метод обновляет члены **кбформат** и **пбформат** структуры **\_ \_ типа мультимедиа AM** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>мтипе. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиатипе**](cmediatype.md)
</dt> </dl>

 

 




