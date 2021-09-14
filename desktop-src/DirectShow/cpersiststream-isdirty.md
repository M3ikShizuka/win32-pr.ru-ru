---
description: Указывает, изменился ли объект со времени последнего сохранения в текущем потоке.
ms.assetid: 69840be6-062e-4505-8381-ea04e822c660
title: Метод Кперсистстреам. IsDirty (Пстреам. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPersistStream.IsDirty
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4f3bc57998b63ece5ca32543fc00d1d3b5b4389b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054662"
---
# <a name="cpersiststreamisdirty-method"></a>Кперсистстреам. IsDirty, метод

Указывает, изменился ли объект со времени последнего сохранения в текущем потоке.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IsDirty();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение \_ ОК, если для фильтра требуется сохранение, и \_ false, если нет необходимости сохранять.

## <a name="remarks"></a>Комментарии

Эта функция члена реализует метод **IPersistStream:: IsDirty** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>пстреам. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кперсистстреам**](cpersiststream.md)
</dt> </dl>

 

 




