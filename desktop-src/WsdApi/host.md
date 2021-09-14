---
description: Определяет элементы ServiceID и Types для узла службы.
ms.assetid: 95066c04-5bdc-4c97-98b8-1da9928d9395
title: ведущий элемент
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c9f051f6665715ecaa519a060e18a3cbf4912210
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058319"
---
# <a name="host-element"></a>ведущий элемент

Определяет элементы [**ServiceID**](serviceid.md) и [**types**](types.md) для узла службы.

## <a name="usage"></a>Использование

``` syntax
<host>
  child elements
</host>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                   | Описание                                                                 |
|-------------------------------------------|-----------------------------------------------------------------------------|
| [**ServiceID**](serviceid.md)<br/> | Определяет идентификатор службы для узла службы.<br/> <br/> |
| [**Типы**](types.md)<br/>         | Определяет список полных имен XSD.<br/> <br/>               |



### <a name="child-element-sequence"></a>Последовательность дочерних элементов

``` syntax
(
  ServiceID, 
  Types
)
```

## <a name="parent-elements"></a>Родительские элементы



| Элемент                                         | Описание                                                                   |
|-------------------------------------------------|-------------------------------------------------------------------------------|
| [**хостметадата**](hostmetadata.md)<br/> | Метаданные размещения для реализуемого устройства.<br/> <br/> |



## <a name="element-information"></a>Сведения об элементе



| Метка | Значение |
|-------------------------------------|---------------|
| Минимальная поддерживаемая система<br/> | Windows Vista |
| Может быть пустым                        | Нет            |



 

 




