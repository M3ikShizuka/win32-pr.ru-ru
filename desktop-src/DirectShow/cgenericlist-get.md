---
description: Метод Get извлекает элемент в указанной позиции.
ms.assetid: cafa4083-96e6-4ed3-afbc-5828b7f1c5be
title: Метод Кженериклист. Get (Вкслист. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList.Get
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 02af7d57d2219e6eb0506a8ab11521b4cf3570eb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055597"
---
# <a name="cgenericlistget-method"></a>Кженериклист. Get, метод

`Get`Метод извлекает элемент в указанной позиции.

## <a name="syntax"></a>Синтаксис


```C++
OBJECT* Get(
   POSITION pos
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pos* 
</dt> <dd>

Индикатор позиции для извлекаемого элемента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на объект типа **Object** (тип шаблона).

## <a name="remarks"></a>Комментарии

Если *POS* имеет **значение NULL**, метод возвращает **значение NULL**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вкслист. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




