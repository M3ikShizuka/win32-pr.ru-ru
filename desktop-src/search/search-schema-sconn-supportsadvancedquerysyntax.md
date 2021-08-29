---
description: Элемент Boolean &lt; суппортсадванцедкуерисинтакс &gt; указывает, поддерживает ли поставщик поиска расширенный синтаксис запроса. Значение по умолчанию – false. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.
ms.assetid: d4aef1f1-63c8-4e9a-9e22-5efbb8c523b2
title: Элемент Суппортсадванцедкуерисинтакс (схема соединителя поиска)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 432c6917ccf03ddf4a00f30029e01b9075309c65
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122880433"
---
# <a name="supportsadvancedquerysyntax-element-search-connector-schema"></a>Элемент Суппортсадванцедкуерисинтакс (схема соединителя поиска)

Элемент Boolean &lt; суппортсадванцедкуерисинтакс &gt; указывает, поддерживает ли поставщик поиска [Расширенный синтаксис запроса](-search-3x-advancedquerysyntax.md). Значение по умолчанию – false. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- supportsAdvancedQuerySyntax -->
    <xs:complexType name="searchConnectorDescriptionType">
        <xs:all>
            ...
            <xs:element name="supportsAdvancedQuerySyntax" type="xs:boolean" default="false" minOccurs="0"/>
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

Значение `true` указывает, что поставщик поиска поддерживает расширенный синтаксис запроса, отправленный в поисковых запросах.

## <a name="example"></a>Пример


```
<?xml version="1.0" encoding="UTF-8"?>
<searchConnectorDescription xmlns="http://schemas.microsoft.com/windows/2009/searchConnector">
    ...
    <supportsAdvancedQuerySyntax>true</supportsAdvancedQuerySyntax>
    ...
</searchConnectionDescription>
```



 

 



