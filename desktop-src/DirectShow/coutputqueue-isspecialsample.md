---
description: Метод ИсспеЦиалсампле определяет, являются ли данные в очереди управляющим сообщением.
ms.assetid: 33d9c7a2-3046-45a5-a9f5-8f33a03bbcdd
title: Каутпуткуеуе. ИсспеЦиалсампле, метод (Аутпутк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- COutputQueue.IsSpecialSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: cc57847d6a977c740bbf50bae220a89b0ed6fab1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246766"
---
# <a name="coutputqueueisspecialsample-method"></a>Каутпуткуеуе. ИсспеЦиалсампле, метод

`IsSpecialSample`Метод определяет, являются ли данные в очереди управляющим сообщением.

## <a name="syntax"></a>Синтаксис


```C++
BOOL IsSpecialSample(
   IMediaSample *pSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псампле* 
</dt> <dd>

Указатель на элемент в очереди.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если *псампле* является управляющим сообщением, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Метод [**каутпуткуеуе:: QueueSample**](coutputqueue-queuesample.md) может получать управляющие сообщения в дополнение к примерам мультимедиа. Управляющее сообщение — это определенная константа (приведение к \_ типу Long PTR), которая указывает потоку выполнить действие. Управляющие сообщения не содержат данных мультимедиа. Дополнительные сведения см. в разделе **каутпуткуеуе:: QueueSample**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




