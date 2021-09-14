---
title: Сложный тип Темплателисттипе
description: Определяет список шаблонов, указывающих данные, включаемые в события. | Сложный тип Темплателисттипе
ms.assetid: 7f676746-6773-4ae2-8330-60d432c29e3a
keywords:
- Журнал событий сложных типов Темплателисттипе
topic_type:
- apiref
api_name:
- TemplateListType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a60b31fd88d05f00229f27a616a29483a29bd49d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242731"
---
# <a name="templatelisttype-complex-type"></a>Сложный тип Темплателисттипе

Определяет список шаблонов, указывающих данные, включаемые в события.

``` syntax
<xs:complexType name="TemplateListType">
    <xs:sequence>
        <xs:element name="template"
            type="TemplateItemType"
            minOccurs="0"
            maxOccurs="unbounded"
         />
    </xs:sequence>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                   | Тип                                                                         | Описание                                                           |
|---------------------------------------------------------------------------|------------------------------------------------------------------------------|-----------------------------------------------------------------------|
| [**шаблон**](eventmanifestschema-template-templatelisttype-element.md) | [**темплатеитемтипе**](eventmanifestschema-templateitemtype-complextype.md) | Шаблон, определяющий данные, включаемые в событие.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





