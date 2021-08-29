---
description: Метод Reset сбрасывает объект, чтобы он мог получить больше данных.
ms.assetid: 7074ed71-1650-4b21-a9a2-ad74d0e3e882
title: Метод Каутпуткуеуе. Reset (Аутпутк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- COutputQueue.Reset
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4129730ae3ce2f3a95db41d8bc65025c3195056cbd4a1afddbfeb83d9bb33ea9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119073658"
---
# <a name="coutputqueuereset-method"></a>Каутпуткуеуе. Reset, метод

`Reset`Метод сбрасывает объект, чтобы он мог получить больше данных.

## <a name="syntax"></a>Синтаксис


```C++
void Reset();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод сбрасывает переменную члена [**каутпуткуеуе:: m \_ HR**](coutputqueue-m-hr.md) в значение S \_ ОК. Объект может снова получать примеры мультимедиа; Например, после операции очистки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




