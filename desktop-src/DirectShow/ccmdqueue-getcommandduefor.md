---
description: Метод Жеткомманддуефор извлекает отложенную команду, которая запланирована в указанное время.
ms.assetid: f8a2f9ae-f359-4429-aca5-021b6fe2aa93
title: Ккмдкуеуе. Жеткомманддуефор, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CCmdQueue.GetCommandDueFor
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c290c5fac2bdf5fd0591a0b088189182638f6b796506361a288fadffe695a85d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119757344"
---
# <a name="ccmdqueuegetcommandduefor-method"></a>Ккмдкуеуе. Жеткомманддуефор, метод

`GetCommandDueFor`Метод получает отложенную команду, которая запланирована в указанное время.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT GetCommandDueFor(
   REFERENCE_TIME   tStream,
   CDeferredCommand **ppCmd
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тстреам* 
</dt> <dd>

Время, для которого запланирована команда.

</dd> <dt>

*ppCmd* 
</dt> <dd>

Адрес указателя на отложенную команду, которая должна быть выполнена в момент, указанный в параметре *тстреам* .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает VFW \_ E \_ не \_ найдено, если нет ни одной команды; в противном случае возвращается значение S \_ ОК.

## <a name="remarks"></a>Remarks

Эта функция-член принимает потоковое время и возвращает отложенную команду, запланированную в это время. Фактическое смещение времени потока вычисляется при выполнении очереди команд. Команды остаются в очереди до выполнения или отмены. Эта функция члена не будет блокироваться.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ккмдкуеуе**](ccmdqueue.md)
</dt> </dl>

 

 




