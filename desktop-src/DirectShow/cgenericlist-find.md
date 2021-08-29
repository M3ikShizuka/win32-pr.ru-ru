---
description: Метод Find извлекает первую позицию, содержащую указанный элемент.
ms.assetid: 8e2a3e5d-96e6-4f40-8e2a-4dc8c21088cd
title: Метод Кженериклист. Find (Вкслист. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList.Find
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e36ea355fed2099769b375abc23aedd1795d6b54b4db3584296070fbfe496b8e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119813804"
---
# <a name="cgenericlistfind-method"></a>Кженериклист. Find, метод

`Find`Метод извлекает первую позицию, содержащую указанный элемент.

## <a name="syntax"></a>Синтаксис


```C++
POSITION Find(
   OBJECT *pObj
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*побж* 
</dt> <dd>

Указатель на объект типа **Object** (тип шаблона).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение позиции или **значение NULL** , если элемент отсутствует в списке.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вкслист. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




