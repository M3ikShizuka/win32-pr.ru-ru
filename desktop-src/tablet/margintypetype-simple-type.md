---
description: Определяет тип, содержащий допустимые значения для атрибута Type элемента Margin.
ms.assetid: 5448ead5-0249-4cc7-9f2a-d2181e2af734
title: Простой тип Маргинтипетипе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- MarginTypeType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: b1996b99729e177f7012db097644807a2bf7052f231e089052d5244b20d016ae
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119031692"
---
# <a name="margintypetype-simple-type"></a>Простой тип Маргинтипетипе

Определяет тип, содержащий допустимые значения для атрибута **Type** [элемента Margin](margin-element.md).

``` syntax
<xs:simpleType name="MarginTypeType">
    <xs:restriction
        base="string"
    >
        <xs:pattern
            value="Left|Right"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="patterns"></a>Шаблоны

Простой тип **маргинтипетипе** — это **строка** , которая ограничена следующим шаблоном:

-   `Left|Right`

## <a name="remarks"></a>Remarks

Допустимые значения для атрибута **Type** [элемента Margin](margin-element.md) : Left и right.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                     |



 

 




