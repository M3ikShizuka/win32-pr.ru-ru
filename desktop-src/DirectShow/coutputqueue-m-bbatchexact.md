---
description: Флаг, указывающий, доставляет ли объект выборки в точных пакетах.
ms.assetid: 1a37c78f-4499-4ebb-92b4-b71ba3ff1a02
title: 'Элемент Каутпуткуеуе:: m_bBatchExact (Аутпутк. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_bBatchExact
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a5f38d8a0e7335025688f52015ff9ed4d4892820
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246754"
---
# <a name="coutputqueuem_bbatchexact-member"></a>Элемент Каутпуткуеуе:: m \_ ббатчексакт

Флаг, указывающий, доставляет ли объект выборки в точных пакетах.

## <a name="syntax"></a>Синтаксис


```C++
const BOOL m_bBatchExact;
```



## <a name="remarks"></a>Remarks

Если значение равно **true**, объект ожидает, пока не будет выполнен полный пакет примеров мультимедиа перед доставкой. В противном случае он доставляет образцы по мере их поступления. Переменная члена [**каутпуткуеуе:: m \_ лбатчсизе**](coutputqueue-m-lbatchsize.md) определяет размер пакета.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




