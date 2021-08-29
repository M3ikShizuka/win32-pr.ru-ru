---
description: Элемент логического типа <isSearchOnlyItem> определяет, поддерживает ли поставщик поиска режим просмотра в дополнение к режиму поиска. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.
ms.assetid: eec1b735-ae78-48ef-8ebf-05b9fd038963
title: Элемент Иссеарчонлитем (схема соединителя поиска)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5ff06fa562db4fc4ada5252b9c7e61d0816c5acdf9336a5fd46503d445d81b34
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119844674"
---
# <a name="issearchonlyitem-element-search-connector-schema"></a>Элемент Иссеарчонлитем (схема соединителя поиска)

Элемент логического типа <isSearchOnlyItem> определяет, поддерживает ли поставщик поиска режим просмотра в дополнение к режиму поиска. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- isSearchOnlyItem -->
    <xs:complexType name="searchConnectorDescriptionType">
        <xs:all>
            <xs:element name="isSearchOnlyItem" type="xs:boolean" default="false" minOccurs="0"/>
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



 

## <a name="remarks"></a>Remarks

Значение `true` указывает, что пользователи не могут просматривать расположение соединителя поиска. Значение `false` указывает, что пользователи могут просматривать расположение соединителя поиска.

## <a name="example"></a>Пример


```
<?xml version="1.0" encoding="UTF-8"?>
<searchConnectorDescription xmlns="http://schemas.microsoft.com/windows/2009/searchConnector">
    ...
    <isSearchOnlyItem>true</isSearchOnlyItem>
    ...
</searchConnectionDescription>
```



 

 



