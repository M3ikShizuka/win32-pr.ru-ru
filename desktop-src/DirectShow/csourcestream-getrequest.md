---
description: Метод GetNext ожидает следующий запрос потока.
ms.assetid: 2938374b-174f-4276-98a2-20a084bd9bbd
title: Метод Ксаурцестреам. WebRequest (Source. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceStream.GetRequest
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 3f45e6f6cf269f7aca6741d8e1c150c7054b07f1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065696"
---
# <a name="csourcestreamgetrequest-method"></a>Ксаурцестреам. метод запроса

`GetRequest`Метод ожидает следующего запроса потока.

## <a name="syntax"></a>Синтаксис


```C++
Command GetRequest();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает следующий запрос потока.

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**камсреад:: WebRequest**](camthread-getrequest.md) . Возвращаемое значение приводится к следующему перечислимому типу:


```C++
enum Command {CMD_INIT, CMD_PAUSE, CMD_RUN, CMD_STOP, CMD_EXIT};
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Source. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурцестреам**](csourcestream.md)
</dt> </dl>

 

 




