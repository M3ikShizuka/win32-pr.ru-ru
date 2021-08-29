---
description: 'Метод Исдисконтинуити определяет, представляет ли этот образец разрыв в потоке данных. Этот метод реализует метод Имедиасампле:: Исдисконтинуити.'
ms.assetid: 125b4a86-bd26-4539-a9ab-281f1aed1836
title: Кмедиасампле. Исдисконтинуити, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaSample.IsDiscontinuity
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: db45e2921e04d798c9b2a155472843e7d82c25b90e582c5895dd3fa57962c801
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119832254"
---
# <a name="cmediasampleisdiscontinuity-method"></a>Кмедиасампле. Исдисконтинуити, метод

`IsDiscontinuity`Метод определяет, представляет ли этот образец разрыв в потоке данных. Этот метод реализует метод [**имедиасампле:: исдисконтинуити**](/windows/desktop/api/Strmif/nf-strmif-imediasample-isdiscontinuity) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IsDiscontinuity();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК, если образец является перерывом в потоке данных, и \_ false в противном случае.

## <a name="remarks"></a>Remarks

Значение этого свойства указывается в переменной члена [**кмедиасампле:: m \_ dwFlags**](cmediasample-m-dwflags.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиасампле**](cmediasample.md)
</dt> </dl>

 

 




