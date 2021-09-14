---
description: 'Метод Жетрекуессандле извлекает дескриптор события, сигнального методом Камсреад:: Каллворкер.'
ms.assetid: 6e4496ae-a635-4b55-ae7a-31748f21068b
title: Камсреад. Жетрекуессандле, метод (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAMThread.GetRequestHandle
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 051a6a3e3daed1dae6df3bdbb42e36f07b852d85
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145178"
---
# <a name="camthreadgetrequesthandle-method"></a>Камсреад. Жетрекуессандле, метод

`GetRequestHandle`Метод получает дескриптор события, сигнальное методом [**камсреад:: каллворкер**](camthread-callworker.md) .

## <a name="syntax"></a>Синтаксис


```C++
HANDLE GetRequestHandle() const;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер события.

## <a name="remarks"></a>Remarks

Класс Камевент сохраняет закрытое событие ручного сброса, которое задается Каллворкер и сбрасывается методом [**камсреад:: Reply**](camthread-reply.md) .

При вызове функции, такой как WaitForMultipleObjects, используйте Жетрекуессандле для получения маркера события.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камсреад**](camthread.md)
</dt> </dl>

 

 




