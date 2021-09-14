---
description: Метод GetNext ожидает следующий запрос.
ms.assetid: 9f275ee6-cb78-455a-b924-7337c8d2a6dd
title: Метод Камсреад. WebRequest (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAMThread.GetRequest
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 506707bc78583fd9729ad28fb5507b82bee5e670
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145181"
---
# <a name="camthreadgetrequest-method"></a>Камсреад. метод запроса

`GetRequest`Метод ожидает следующего запроса.

## <a name="syntax"></a>Синтаксис


```C++
DWORD GetRequest();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение, определяемое производным классом.

## <a name="remarks"></a>Remarks

Этот метод блокируется до тех пор, пока другой поток не вызовет метод [**камсреад:: каллворкер**](camthread-callworker.md) . Затем возвращается параметр, который был передан в Каллворкер. Вызовите метод [**камсреад:: Reply**](camthread-reply.md) , чтобы освободить поток запроса.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камсреад**](camthread.md)
</dt> </dl>

 

 




