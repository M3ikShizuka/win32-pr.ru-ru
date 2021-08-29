---
description: Шаблон класса Кженериклист, реализующий список, зависящий от типа. Дополнительные сведения см. в разделе Кбаселист.
ms.assetid: 69067530-3a7d-4731-8ac6-9d02dbba8440
title: Класс Кженериклист (Вкслист. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 79bbc003770d7fec94af93a54386bccbfbd00c4cd2a8b3f9a8ff81e14aa7a6ac
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119999424"
---
# <a name="cgenericlist-class"></a>Класс Кженериклист

![Иерархия классов кженериклист](images/list01.png)

`CGenericList`Шаблон класса, реализующий список, зависящий от типа. Дополнительные сведения см. в разделе [**кбаселист**](cbaselist.md).

Чтобы использовать этот шаблон, объявите переменную типа `CGenericList` с аргументом шаблона, который определяет тип объекта в списке. Например, следующая инструкция объявляет список объектов [**кбасефилтер**](cbasefilter.md) :


```
CGenericList<CBaseFilter> myFilterList("Filters"); 
```



Для удобства Вкслист. h определяет следующие типы списков:

``` syntax
typedef CGenericList<CBaseObject> CBaseObjectList;
typedef CGenericList<IUnknown> CBaseInterfaceList;
```



| Открытые методы                                          | Описание                                                              |
|---------------------------------------------------------|--------------------------------------------------------------------------|
| [**кженериклист**](cgenericlist-cgenericlist.md)       | Метод конструктора.                                                      |
| [**~ Кженериклист**](cgenericlist--cgenericlist.md)     | Метод деструктора.                                                       |
| [**жесеадпоситион**](cgenericlist-getheadposition.md) | Извлекает позицию первого элемента в списке.                    |
| [**жеттаилпоситион**](cgenericlist-gettailposition.md) | Извлекает позицию последнего элемента списка.                     |
| [**GetCount**](cgenericlist-getcount.md)               | Возвращает количество элементов в списке.                               |
| [**GetNext**](cgenericlist-getnext.md)                 | Извлекает элемент в указанной позиции и перемещает позицию. |
| [**Получить**](cgenericlist-get.md)                         | Извлекает элемент в указанной позиции.                            |
| [**Вышлем**](cgenericlist-gethead.md)                 | Извлекает элемент в заголовке списка.                              |
| [**ремовехеад**](cgenericlist-removehead.md)           | Удаляет первый элемент из списка.                                      |
| [**ремоветаил**](cgenericlist-removetail.md)           | Удаляет последний элемент в списке.                                       |
| [**Отменит**](cgenericlist-remove.md)                   | Удаляет элемент по указанному положению.                              |
| [**аддбефоре**](cgenericlist-addbefore.md)             | Вставляет элемент или список до указанной позиции.                   |
| [**аддафтер**](cgenericlist-addafter.md)               | Вставляет элемент или список после указанной позиции.                    |
| [**аддхеад**](cgenericlist-addhead.md)                 | Добавляет элемент или список в начало списка.                           |
| [**AddTail**](cgenericlist-addtail.md)                 | Добавляет элемент или список в конец списка.                          |
| [**Поиск**](cgenericlist-find.md)                       | Извлекает первую позицию, содержащую указанный элемент.              |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вкслист. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




