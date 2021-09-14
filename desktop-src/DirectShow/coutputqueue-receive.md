---
description: Метод Receive доставляет пример носителя во входной ПИН-код.
ms.assetid: a8ee0988-8955-48d0-be1b-24eea72d560d
title: Метод Каутпуткуеуе. Receive (Аутпутк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- COutputQueue.Receive
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 0ce8a0d44730fa35b38cf6d738edd26168284a46
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054683"
---
# <a name="coutputqueuereceive-method"></a>Каутпуткуеуе. Receive, метод

`Receive`Метод доставляет пример носителя во входной ПИН-код.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Receive(
   IMediaSample *pSample
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псампле* 
</dt> <dd>

Указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) образца.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Возможные значения включают в себя, показанные в следующей таблице.



| Код возврата                                                                             | Описание                                                                   |
|-----------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| <dl> <dt>**S \_ false**</dt> </dl> | Перед обработкой этого примера получено уведомление о завершении потока.<br/> |
| <dl> <dt>**\_ОК**</dt> </dl>    | Успешно.<br/>                                                           |



 

## <a name="remarks"></a>Комментарии

Этот метод вызывает метод [**каутпуткуеуе:: рецеивемултипле**](coutputqueue-receivemultiple.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




