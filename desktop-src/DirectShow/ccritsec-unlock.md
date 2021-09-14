---
description: Метод Unlock разблокирует объект критической секции.
ms.assetid: 61811e0e-df77-48e9-96d5-b7dff8c8db9b
title: Метод Ккритсек. Unlock (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CCritSec.Unlock
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ca84ce452d71d0d3111039d7a95d8f5dd3155058
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053572"
---
# <a name="ccritsecunlock-method"></a>Ккритсек. Unlock, метод

Метод **Unlock** разблокирует объект критической секции.

## <a name="syntax"></a>Синтаксис


```C++
void Unlock();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Этот метод вызывает функцию [**LeaveCriticalSection**](/windows/desktop/api/synchapi/nf-synchapi-leavecriticalsection) . Вызывайте этот метод один раз для каждого вызова метода [**ккритсек:: Lock**](ccritsec-lock.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ккритсек**](ccritsec.md)
</dt> </dl>

 

