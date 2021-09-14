---
title: Сложный тип Намедвалуе
description: Определяет имя, связанное со значением в паре "имя-значение".
ms.assetid: 5e3ce01a-9be6-4f12-be02-42065aba46cd
keywords:
- планировщик задач сложного типа Намедвалуе
topic_type:
- apiref
api_name:
- namedValue
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 39d6990194350dcc032d42838f30bdd7339b0d38
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886544"
---
# <a name="namedvalue-complex-type"></a>Сложный тип Намедвалуе

Определяет имя, связанное со значением в паре "имя-значение".

``` syntax
<xs:complexType name="namedValue">
    <xs:simpleContent>
        <xs:extension
            base="nonEmptyString"
        >
            <xs:attribute name="name"
                type="nonEmptyString"
                use="required"
             />
        </xs:extension>
    </xs:simpleContent>
</xs:complexType>
```

## <a name="attributes"></a>Атрибуты



| Имя | Тип                                                                    | Описание                                                                          |
|------|-------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| name | [**нонемптистринг**](taskschedulerschema-nonemptystring-simpletype.md) | Указывает имя, связанное со значением в паре «имя-значение». <br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





