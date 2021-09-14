---
description: Метод Reply отвечает на запрос.
ms.assetid: 90e91b99-6a1c-46a2-b83d-eba483f1832a
title: Метод Камсреад. Reply (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAMThread.Reply
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 5e86e0bc0155e527aa11c26531ae5608e6828362
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145161"
---
# <a name="camthreadreply-method"></a>Камсреад. Reply, метод

`Reply`Метод отвечает на запрос.

## <a name="syntax"></a>Синтаксис


```C++
void Reply(
   DWORD dw
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*dw* 
</dt> <dd>

Значение, возвращаемое методом [**камсреад:: каллворкер**](camthread-callworker.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Метод Каллворкер блокируется до вызова этого метода. Параметр *DW* предоставляет возвращаемое значение для каллворкер. Вызовите этот метод в процедуре потока после получения запроса, чтобы освободить поток запроса.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камсреад**](camthread.md)
</dt> </dl>

 

 




