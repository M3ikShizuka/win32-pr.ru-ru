---
description: Метод Стреамингсреадусингаутпутпин определяет, выполняет ли поток потоковую операцию с закреплением.
ms.assetid: b6432a11-4e8b-4eb4-ad8e-aaff9398641b
title: Кдинамикаутпутпин. Стреамингсреадусингаутпутпин, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDynamicOutputPin.StreamingThreadUsingOutputPin
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 797dcb94e227861642de2a05e6edf24f675bb4e7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054753"
---
# <a name="cdynamicoutputpinstreamingthreadusingoutputpin-method"></a>Кдинамикаутпутпин. Стреамингсреадусингаутпутпин, метод

Метод Стреамингсреадусингаутпутпин определяет, выполняет ли поток потоковую операцию с закреплением.

## <a name="syntax"></a>Синтаксис


```C++
virtual bool StreamingThreadUsingOutputPin();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если поток выполняет потоковую операцию над закреплением. В противном случае возвращает **значение false**.

## <a name="remarks"></a>Комментарии

Если какие-либо потоки успешно возвращали метод [**кдинамикаутпутпин:: стартусингаутпутпин**](cdynamicoutputpin-startusingoutputpin.md) и не выполнили соответствующий вызов метода [**Кдинамикаутпутпин:: стопусингаутпутпин**](cdynamicoutputpin-stopusingoutputpin.md) , этот метод возвращает **значение true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдинамикаутпутпин**](cdynamicoutputpin.md)
</dt> </dl>

 

 




