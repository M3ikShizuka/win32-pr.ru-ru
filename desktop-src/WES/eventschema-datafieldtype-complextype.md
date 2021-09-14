---
title: сложный тип DataType (Windows журнал событий)
description: Определяет элемент данных.
ms.assetid: f3b7de63-1ac1-429d-9e36-1f13c26c9618
keywords:
- Журнал событий сложного типа DataType
topic_type:
- apiref
api_name:
- DataType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9d3ac6e545cbe8567bbe041568c442f762743ad0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242596"
---
# <a name="datatype-complex-type"></a>Сложный тип DataType

Определяет элемент данных.

``` syntax
<xs:complexType name="DataType">
    <xs:simpleContent>
        <xs:extension
            base="string"
        >
            <xs:attribute name="Name"
                type="string"
                use="optional"
             />
            <xs:attribute name="Type"
                type="QName"
                use="optional"
             />
        </xs:extension>
    </xs:simpleContent>
</xs:complexType>
```

## <a name="attributes"></a>Атрибуты



| Имя | Тип   | Описание                                                                                                                                                              |
|------|--------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Название | строка | Имя элемента данных, определенного в шаблоне (см. сложный тип [**темплатеитемтипе**](eventmanifestschema-templateitemtype-complextype.md) ).<br/> |
| Тип | QName  | Не используется.<br/>                                                                                                                                                     |



## <a name="remarks"></a>Remarks

Элемент данных может быть элементом данных верхнего уровня или элементом данных в структуре.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





