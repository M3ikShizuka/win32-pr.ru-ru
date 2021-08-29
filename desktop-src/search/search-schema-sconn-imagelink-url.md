---
description: '&lt;Элемент URL &gt; задает URL-адрес эскиза для этого соединителя поиска. Если &lt; имажелинк &gt; существует, этот элемент является обязательным. У него нет дочерних элементов и атрибутов.'
ms.assetid: addb2614-9f4f-4cab-a678-b6020b8c4648
title: Элемент URL-адреса Имажелинк (схема соединителя поиска)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 011142e509d34f4942027b90625c9692c7aa87ff
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122882405"
---
# <a name="imagelink-url-element-search-connector-schema"></a>Элемент URL-адреса Имажелинк (схема соединителя поиска)

&lt;Элемент URL &gt; задает URL-адрес эскиза для этого соединителя поиска. Если &lt; имажелинк &gt; существует, этот элемент является обязательным. У него нет дочерних элементов и атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- url -->
    <xs:complexType name="searchConnectorDescriptionType">
        <xs:all>
            ...
            <xs:element name="imageLink" minOccurs="0">
                <xs:complexType>
                    <xs:sequence>
                        <xs:element name="url" type="xs:anyURI"/>
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
            ...
        </xs:all>
        <xs:attribute name="publisher" type="xs:string"/>
        <xs:attribute name="product" type="xs:string"/>
    </xs:complexType>
```



## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                                   | Дочерние элементы |
|----------------------------------------------------------------------------------|----------------|
| [Элемент Имажелинк (схема соединителя поиска)](search-schema-sconn-imagelink.md) |                |



 

## <a name="remarks"></a>Комментарии

Значением может быть путь к локальной файловой системе или URL-адрес. файл изображения может быть любым из базовых типов образов, поддерживаемых Windows 7 (PNG, BMP, JPG, GIF).

## <a name="example-of-an-imagelinkurl-element"></a>Пример элемента Имажелинкурл


```
<imageLink>
    <imageLinkurl>%ProgramFiles%\Example\examplethumbnail.jpg</imageLinkurl>
</imageLink>
```



 

 



