---
description: Метод AddTail добавляет элемент в конец списка.
ms.assetid: e365a23e-7447-42ec-b836-21dd68962db1
title: Кженериклист. AddTail, метод (Вкслист. h) — параметр Побж
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList.AddTail
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 614a2f26349834c01f0a3e7587eae28c41e546a0585ef603af0265ea35c187d9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120055614"
---
# <a name="cgenericlistaddtail-method-wxlisth---pobj-parameter"></a>Кженериклист. AddTail, метод (Вкслист. h) — параметр Побж

`AddTail`Метод добавляет элемент в конец списка.

## <a name="syntax"></a>Синтаксис


```C++
POSITION AddTail(
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

Возвращает значение позиции для новой позиции хвоста. Если метод завершается с ошибкой, возвращается **значение NULL**.

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|-|-|
| Заголовок | вкслист. h (включает Потоки. h) |
| Библиотека| Стрмбасе. lib (розничные сборки); Стрмбасд. lib (отладочные сборки) |

## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




