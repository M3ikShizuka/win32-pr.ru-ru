---
description: Доменное имя поставщика домашней сети устройства, идентифицирующее оператора сети.
ms.assetid: 7676e1d8-a414-401f-989c-9f60068b92d8
title: Имя_домена (Hotspot2), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DomainName
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 670fc91771ee0a47cd7f16f617d052df2e567b2d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245515"
---
# <a name="domainname-hotspot2-element"></a>Имя_домена (Hotspot2), элемент

Доменное имя поставщика домашней сети устройства, идентифицирующее оператора сети.

``` syntax
<xs:element name="DomainName"
    minOccurs="0"
>
    <xs:simpleType>
        <xs:restriction
            base="string"
        >
            <xs:minLength
                value="1"
             />
            <xs:maxLength
                value="255"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент определяется элементом [**Hotspot2**](wlan-profileschema-hotspot2-element.md) .

 

 



