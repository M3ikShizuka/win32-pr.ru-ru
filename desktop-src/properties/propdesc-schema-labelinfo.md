---
description: Указывает способ отображения меток свойства.
ms.assetid: 9317aff9-abdd-46c2-aaff-62861925713b
title: лабелинфо
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8d2d358270bfdf231f990feee54d90f6f39f16fa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252268"
---
# <a name="labelinfo"></a>лабелинфо

Указывает способ отображения меток свойства. Для каждого элемента [пропертидескриптион](./propdesc-schema-propertydescription.md) должен быть только один элемент [лабелинфо]() .

При наличии нескольких элементов используется последний из них. Если элемент [лабелинфо]() не указан, метка свойства не отображается; Однако это обычно является дефектом.

## <a name="syntax"></a>Синтаксис


```
<!-- labelInfo -->
<xs:element name="labelInfo">
    <xs:complexType>
        <xs:attribute name="label" type="xs:string"/>
        <xs:attribute name="sortDescription">
            <xs:simpleType>
                <xs:restriction base="xs:string">
                    <xs:enumeration value="General"/>
                    <xs:enumeration value="AToZ"/>
                    <xs:enumeration value="LowestHighest"/>
                    <xs:enumeration value="OldestNewest"/>
                    <xs:enumeration value="SmallestLargest"/>
                </xs:restriction>
            </xs:simpleType>
        </xs:attribute>
        <xs:attribute name="invitationText" type="xs:string"/>
        <xs:attribute name="hideLabel" type="xs:boolean" default="false"/>
    </xs:complexType>
</xs:element>
```



## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                   | Дочерние элементы |
|------------------------------------------------------------------|----------------|
| [пропертидескриптион](./propdesc-schema-propertydescription.md) | None           |



 

## <a name="attributes"></a>Атрибуты




| Атрибут | Описание | 
|-----------|-------------|
| label | Общедоступный. Необязательный элемент. Метка, отображаемая в пользовательском интерфейсе (например, метка столбца сведений или панель предварительного просмотра). Синтаксис позволяет получить прямую отображаемую строку или ссылку на непрямо отображаемую строку. Используйте строку с косвенным отображением, так как она может быть локализована. <a href="/windows/win32/api/propsys/nf-propsys-ipropertydescription-getdisplayname"><strong>Ипропертидескриптион::</strong></a> Возвращает разрешенное отображаемое имя. | 
| сортдескриптион | Необязательный элемент. Указывает строки, предлагаемые в качестве параметров сортировки. <a href="/windows/win32/api/propsys/nf-propsys-ipropertydescription-getsortdescription"><strong>Ипропертидескриптион:: жетсортдескриптион</strong></a> возвращает это описание сортировки. Следующие значения предоставляют соответствующие строки пользовательского интерфейса.<ul><li>Общие: "Сортировать по возрастанию"/"Сортировать"</li><li>Атоз: "а сверху"/"Z поверх остальных"</li><li>Ловессигхест: "низший поверх"/"самый высокий на вершине"</li><li>Олдестневест: "самые старые сверху"/"самые новые в начале"</li><li>Смаллестларжест: "наименьший на вершине"/"самый крупный на вершине"</li></ul> | 
| инвитатионтекст | Необязательный параметр. Текст строки справки, отображаемый в качестве инструкции пользователю для элемента управления или подсказки (например, "введите имя автора)". Синтаксис позволяет получить прямую отображаемую строку или ссылку на непрямо отображаемую строку. Используйте строку с косвенным отображением, так как она может быть локализована. <a href="/windows/win32/api/propsys/nf-propsys-ipropertydescription-geteditinvitation"><strong>Ипропертидескриптион:: жетедитинвитатион</strong></a> возвращает Разрешенный текст приглашения. | 
| хиделабел | Необязательный параметр. Значение по умолчанию — «false». Указывает, скрыта ли метка. | 




 

 

 
