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
ms.openlocfilehash: 2f1e7cd3d8758107b9529114a75b3a90527937c6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172019"
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

## <a name="requirements"></a>Требования

| Требование | Значение |
|-|-|
| Заголовок | вкслист. h (включает Потоки. h) |
| Библиотека| Стрмбасе. lib (розничные сборки); Стрмбасд. lib (отладочные сборки) |

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




