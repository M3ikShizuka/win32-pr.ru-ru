---
description: Определяет список, содержащий до пяти атрибутов счетчика.
ms.assetid: d710c3d2-2886-4f1a-bd27-f11451d2f3c6
title: Сложный тип Каунтераттрибутес
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- kbSyntax
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: be740abacc9a10674b98e2c2088f647dfaa26c7cd99c7e55efbfe968731a9a54
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119775424"
---
# <a name="counterattributes-complex-type"></a>Сложный тип Каунтераттрибутес

Определяет список, содержащий до пяти атрибутов счетчика.

``` syntax
<xs:complexType name="counterAttributes">
    <xs:choice
        minOccurs="1"
        maxOccurs="5"
    >
        <xs:element name="counterAttribute"
            type="man:counterAttribute"
         />
    </xs:choice>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент              | Тип                                                                               | Описание                                                                                                |
|----------------------|------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| **каунтераттрибуте** | [**мужчина: Каунтераттрибуте**](performance-counters-counterattribute-complex-type.md) | Атрибут счетчика, указывающий способ отображения данных счетчиков в приложении-потребителе.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




