---
description: Метод Run сообщает поток потоковой передачи для выполнения.
ms.assetid: 9aef7801-dcfb-4597-bccb-5ba19327b2d5
title: Метод Ксаурцестреам. Run (Source. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceStream.Run
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fb7d1d9c86759331127b3db893e05e075d0fffb5988a61935cc28d2e0027ba39
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119823944"
---
# <a name="csourcestreamrun-method"></a>Ксаурцестреам. Run, метод

`Run`Метод оповещает поток потоковой передачи о выполнении.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Run();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Непредвиденное значение: S \_ (ОК или E) \_ .

## <a name="remarks"></a>Remarks

В базовом классе этот метод действует так же, как запрос [**ксаурцестреам::P Аусе**](csourcestream-pause.md) , и не используется.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Source. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурцестреам**](csourcestream.md)
</dt> </dl>

 

 




