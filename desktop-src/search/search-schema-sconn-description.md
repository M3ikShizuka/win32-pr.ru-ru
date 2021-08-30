---
description: Необязательный &lt; &gt; элемент Description задает описание для этого соединителя поиска. Этот элемент не имеет дочерних элементов и не имеет атрибутов.
ms.assetid: 0e9d806c-7dfd-4e7f-8843-15a4e22f317f
title: Элемент Description (схема соединителя поиска)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b0fd7314f29fb6a402416d861069cf048ecfac0c
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122882490"
---
# <a name="description-element-search-connector-schema"></a>Элемент Description (схема соединителя поиска)

Необязательный &lt; &gt; элемент Description задает описание для этого соединителя поиска. Этот элемент не имеет дочерних элементов и не имеет атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- description -->
    <xs:complexType name="searchConnectorDescriptionType">
        <xs:all>
            ...
            <xs:element name="description" type="xs:string" minOccurs="0"/>
            ...
        </xs:all>
        <xs:attribute name="publisher" type="xs:string"/>
        <xs:attribute name="product" type="xs:string"/>
    </xs:complexType>
```



## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                                                                   | Дочерние элементы |
|------------------------------------------------------------------------------------------------------------------|----------------|
| [Элемент Сеарчконнектордескриптионтипе (схема соединителя поиска)](search-schema-searchconnectordescription.md) |                |



 

## <a name="remarks"></a>Комментарии

Описание должно быть понятным для пользователя, так как оно может использоваться во всплывающих подсказках.

## <a name="example"></a>Пример


```
<?xml version="1.0" encoding="UTF-8"?>
<searchConnectorDescription xmlns="https://schemas.adventureworks.com/searchConnector">
    ...
    <description>Search AdventureWorks.com</description>
    ...
</searchConnectionDescription>
```



 

 



