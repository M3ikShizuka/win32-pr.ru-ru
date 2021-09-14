---
title: Сложный тип Локализатионтипе
description: Определяет группу локализованных ресурсов, на которые ссылается манифест. | Сложный тип Локализатионтипе
ms.assetid: fecab4e0-7136-4b13-8c24-bebbad0812e6
keywords:
- Журнал событий сложных типов Локализатионтипе
topic_type:
- apiref
api_name:
- LocalizationType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: cbb6911ea606ea30d8e656f20b4c566d4f6d0e08
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056493"
---
# <a name="localizationtype-complex-type"></a>Сложный тип Локализатионтипе

Определяет группу локализованных ресурсов, на которые ссылается манифест.

``` syntax
<xs:complexType name="LocalizationType">
    <xs:choice
        minOccurs="0"
        maxOccurs="unbounded"
    >
        <xs:element name="resources">
            <xs:complexType>
                <xs:choice
                    minOccurs="0"
                    maxOccurs="unbounded"
                >
                    <xs:element name="stringTable"
                        type="StringTableType"
                     />
                </xs:choice>
                <xs:attribute name="culture"
                    type="string"
                    use="required"
                 />
                <xs:anyAttribute
                    processContents="lax"
                    namespace="##other"
                 />
            </xs:complexType>
        </xs:element>
        <xs:any
            processContents="lax"
            minOccurs="0"
            namespace="##other"
         />
    </xs:choice>
    <xs:attribute name="fallbackCulture"
        type="string"
        default="en-us"
        use="optional"
     />
    <xs:anyAttribute
        processContents="lax"
        namespace="##other"
     />
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                         | Тип                                                                       | Описание                                                                                                         |
|---------------------------------------------------------------------------------|----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| [**источников**](eventmanifestschema-resources-localizationtype-element.md)     |                                                                            | Определяет группу строковых таблиц, содержащих локализованные строки, на которые ссылается манифест.<br/> |
| [**stringTable**](eventmanifestschema-stringtable-localizationtype-element.md) | [**стрингтаблетипе**](eventmanifestschema-stringtabletype-complextype.md) | Определяет список локализованных строк, на которые можно ссылаться в манифесте.<br/>                             |



## <a name="attributes"></a>Атрибуты



| Имя            | Тип   | Описание                                                                                                                                            |
|-----------------|--------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| culture         | строка | Имя языка, определяющее язык и региональные параметры локализованных строк в таблице строк. Например, "en-US" для английского языка (США).<br/> |
| фаллбакккултуре | строка | Не используется.<br/>                                                                                                                                   |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





