---
title: Сложный тип Типелисттипе
description: Определяет типы, используемые в манифесте.
ms.assetid: e7ce0ecf-3bd0-49ab-82c7-dc28fd0e59a2
keywords:
- Журнал событий сложных типов Типелисттипе
topic_type:
- apiref
api_name:
- TypeListType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 61cec902684d7426a5951c12c4b319ae1ce29923
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242722"
---
# <a name="typelisttype-complex-type"></a>Сложный тип Типелисттипе

Определяет типы, используемые в манифесте.

``` syntax
<xs:complexType name="TypeListType">
    <xs:choice
        maxOccurs="unbounded"
    >
        <xs:element name="xmlTypes"
            type="XmlTypeListType"
         />
        <xs:element name="inTypes"
            type="InputTypeListType"
         />
        <xs:any
            processContents="lax"
            namespace="##other"
         />
    </xs:choice>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                               | Тип                                                                           | Описание                                                                                                 |
|-----------------------------------------------------------------------|--------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| [**нетипизированные типы**](eventmanifestschema-intypes-typelisttype-element.md)   | [**инпуттипелисттипе**](eventmanifestschema-inputtypelisttype-complextype.md) | Определяет список входных типов данных.<br/>                                                              |
| [**ксмлтипес**](eventmanifestschema-xmltypes-typelisttype-element.md) | [**ксмлтипелисттипе**](eventmanifestschema-xmltypelisttype-complextype.md)     | Определяет выходные типы списка, которые служба использует для определения способа визуализации входного типа данных.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





