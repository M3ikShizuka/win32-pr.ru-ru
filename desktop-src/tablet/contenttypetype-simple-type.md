---
description: Определяет тип, определяющий допустимые значения для атрибута Type \[ средства чтения журнала элемента содержимого \] .
ms.assetid: f38f7a7e-a517-4156-9c60-e1b6d35baa07
title: Простой тип Контенттипетипе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ContentTypeType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 55297be38dfd75f9ca11bfb6213cd99d52d2a7e0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579494"
---
# <a name="contenttypetype-simple-type"></a>Простой тип Контенттипетипе

Определяет тип, определяющий допустимые значения для атрибута *Type* [ \[ средства \] чтения журнала элемента содержимого](content-element--journal-reader.md).

``` syntax
<xs:simpleType name="ContentTypeType">
    <xs:restriction
        base="string"
    >
        <xs:pattern
            value="Normal|Inert"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="patterns"></a>Шаблоны

Простой тип **контенттипетипе** — это строка, которая ограничена следующим шаблоном:

-   `Normal|Inert`

## <a name="remarks"></a>Remarks

Допустимые значения: "нормальный" и "инерт".

Если тип — «инерт», то содержимое, содержащееся в журнале, является страницей журнала, которая является фоном документа доступным только для чтения и не является редактируемым. Это происходит при создании документа с помощью драйвера принтера составителя заметок журнала.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                     |



 

 




