---
description: Необязательный &lt; элемент логического исдефаултсавелокатион &gt; указывает, следует ли использовать расположение, описанное в соединителе поиска, в качестве расположения для сохранения по умолчанию. Этот элемент не имеет дочерних элементов и не имеет атрибутов.
ms.assetid: 4a33f411-d71e-41d3-b5fd-018a92dceeac
title: Элемент Исдефаултсавелокатион (схема соединителя поиска)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a2a17324f7658290c0eed9345f899f0d9c94f208
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122881905"
---
# <a name="isdefaultsavelocation-element-search-connector-schema"></a>Элемент Исдефаултсавелокатион (схема соединителя поиска)

Необязательный &lt; элемент логического исдефаултсавелокатион &gt; указывает, следует ли использовать расположение, описанное в соединителе поиска, в качестве расположения для сохранения по умолчанию. Этот элемент не имеет дочерних элементов и не имеет атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- isDefaultSaveLocation -->
    <xs:complexType name="searchConnectorDescriptionType">
        <xs:all>
            ...
            <xs:element name="isDefaultSaveLocation" type="xs:boolean" minOccurs="0"/>
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

когда пользователь выбирает сохранение элемента, Windows Explorer сохраняет его в расположении, указанном в &lt; &gt; элементе симплелокатион. Пользователи могут изменить этот параметр, используя диалоговое окно свойств соединителя поиска.

## <a name="example"></a>Пример


```
<?xml version="1.0" encoding="UTF-8"?>
<searchConnectorDescription xmlns="http://schemas.microsoft.com/windows/2009/searchConnector">
    ...
    <isDefaultSaveLocation>true</isDefaultSaveLocation>
    ...
</searchConnectionDescription>
```



 

 



