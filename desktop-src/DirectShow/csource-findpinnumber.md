---
description: Метод Финдпиннумбер извлекает номер указанного пин-кода в фильтре.
ms.assetid: c9366fcc-7b13-4e43-883e-6003c32fadec
title: Метод Ксаурце. Финдпиннумбер (Source. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSource.FindPinNumber
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e8082cb19b275f8ebfebd0f2c9beda0eb9854699bf92f29e9d994ee4391e628f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120084104"
---
# <a name="csourcefindpinnumber-method"></a>Ксаурце. Финдпиннумбер, метод

`FindPinNumber`Метод извлекает номер указанного пин-кода в фильтре.

## <a name="syntax"></a>Синтаксис


```C++
int FindPinNumber(
   IPin *iPin
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ипин* 
</dt> <dd>

Указатель на интерфейс [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin) ПИН-кода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает PIN-код или значение 1, если ПИН-код не найден в этом фильтре. Первый ПИН-код имеет нулевое значение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Source. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурце**](csource.md)
</dt> </dl>

 

 




