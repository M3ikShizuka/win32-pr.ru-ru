---
title: Сложный тип XmlType
description: Определяет фрагмент XML.
ms.assetid: ac6ce2a2-4584-4181-9a39-aceab85d5c51
keywords:
- Журнал событий сложных типов XmlType
topic_type:
- apiref
api_name:
- XmlType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a4a4d71d7f4f2685d6c5f1c0626392c79436b68d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242680"
---
# <a name="xmltype-complex-type"></a>Сложный тип XmlType

Определяет фрагмент XML. Любой экземпляр схемы разрешен; узел верхнего уровня в фрагменте должен содержать атрибут Namespace.

``` syntax
<xs:complexType name="XmlType">
    <xs:sequence>
        <xs:any
            processContents="skip"
            minOccurs="0"
            maxOccurs="unbounded"
            namespace="##other"
         />
    </xs:sequence>
</xs:complexType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





