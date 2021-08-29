---
description: Метод Аддхеад добавляет элемент в начало списка.
ms.assetid: 8f0012b7-bbc2-407c-ae5a-9843c2f692dc
title: Кженериклист. Аддхеад, метод (Вкслист. h) — параметр Побж
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList.AddHead
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 176a31c3acf846c4112e7bcb7bd457872e1e4086b4a8d214ccc7a175e7891feb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119697465"
---
# <a name="cgenericlistaddhead-method-wxlisth---pobj-parameter"></a>Кженериклист. Аддхеад, метод (Вкслист. h) — параметр Побж

`AddHead`Метод добавляет элемент в начало списка.

## <a name="syntax"></a>Синтаксис


```C++
POSITION AddHead(
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

Возвращает значение расположения, указывающее новую головную точку. Если метод завершается ошибкой, возвращается значение **null**.

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|-|-|
| Заголовок | вкслист. h (включает Потоки. h) |
| Библиотека| Стрмбасе. lib (розничные сборки); Стрмбасд. lib (отладочные сборки) |

## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




