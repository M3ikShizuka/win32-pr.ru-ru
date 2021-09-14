---
description: Определяет список структур, содержащих значения счетчиков.
ms.assetid: 6f6b33ed-6440-456c-8379-61a37798c95f
title: Составной тип структур
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- kbSyntax
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: c36de698d1e0eb136f17034e0740851fc751d157
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250567"
---
# <a name="structs-complex-type"></a>Составной тип структур

Определяет список структур, содержащих значения счетчиков.

``` syntax
<xs:complexType name="structs">
    <xs:choice
        minOccurs="1"
        maxOccurs="unbounded"
    >
        <xs:element name="struct"
            type="man:struct"
         />
    </xs:choice>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент    | Тип                                                           | Описание                                                      |
|------------|----------------------------------------------------------------|------------------------------------------------------------------|
| **struct** | [**Man: структура**](performance-counters-struct-complex-type.md) | Имя структуры, содержащей значения счетчика.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




