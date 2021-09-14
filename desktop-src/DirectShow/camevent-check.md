---
description: Метод check проверяет, задано ли событие, без блокировки.
ms.assetid: b8e55798-fd8e-4442-bc35-08887d8a3129
title: Метод Камевент. Check (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAMEvent.Check
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1a112d1b9484acb4d7e9cc2992b8dee629f40e23
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147977"
---
# <a name="cameventcheck-method"></a>Камевент. Check, метод

`Check`Метод проверяет, задано ли событие, без блокировки.

## <a name="syntax"></a>Синтаксис


```C++
BOOL Check();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="remarks"></a>Remarks

Возвращает **значение true** , если событие задано, или **значение false** в противном случае. Этот метод вызывает метод [**камевент:: wait**](camevent-wait.md) с нулевым временем ожидания. Если объект является событием автоматического сброса, этот метод сбрасывает событие.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камевент**](camevent.md)
</dt> </dl>

 

 




