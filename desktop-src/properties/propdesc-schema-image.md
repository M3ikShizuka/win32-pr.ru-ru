---
description: Изображение
ms.assetid: 89893C4E-4F4E-4d85-9623-08607B4383E5
title: Элемент Image (схема описания свойства)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c24ecb1b88b8b724ce299a81281f926972180743
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257496"
---
# <a name="image"></a>Изображение

Для каждого родительского элемента должен быть только один элемент [Image]() .

## <a name="syntax"></a>Синтаксис


```
<!-- image -->
<xs:element name="image">
    <xs:complexType>
        <xs:attribute name="res" use="required">
            <xs:simpleType>
                <xs:restriction base="xs:string">
                    <xs:maxLength value="260"/>
                </xs:restriction>
            </xs:simpleType>
        </xs:attribute>
    </xs:complexType>
</xs:element>
```



## <a name="element-information"></a>Сведения об элементе



| Родительские элементы                                                                  | Дочерние элементы |
|----------------------------------------------------------------------------------|----------------|
| [enum](./propdesc-schema-enum.md), [енумранже](./propdesc-schema-enumrange.md) | Нет           |



 

## <a name="attributes"></a>Атрибуты



| Атрибут | Описание:       |
|-----------|-------------------|
| res       | Общедоступный. Обязательный элемент. |



 

 

 
