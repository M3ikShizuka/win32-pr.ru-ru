---
title: Сложный тип Монсстипе
description: Определяет дочерние элементы и сведения о последовательности для элементов month (Монслидайофвиксчедулетипе) и months (Монслисчедулетипе).
ms.assetid: f1faa67a-2f5f-4a00-a1df-2d44e218278b
keywords:
- планировщик задач сложного типа Монсстипе
topic_type:
- apiref
api_name:
- monthsType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: e6a19000073fd12e05aa915921850264979a0541
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259099"
---
# <a name="monthstype-complex-type"></a>Сложный тип Монсстипе

Определяет дочерние элементы и сведения о последовательности для элементов [**Month (монслидайофвиксчедулетипе)**](taskschedulerschema-months-monthlydayofweekscheduletype-element.md) и [**months (монслисчедулетипе)**](taskschedulerschema-months-monthlyscheduletype-element.md) .

``` syntax
<xs:complexType name="monthsType">
    <xs:all>
        <xs:element name="January"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="February"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="March"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="April"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="May"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="June"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="July"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="August"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="September"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="October"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="November"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="December"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                               | Тип | Описание                                            |
|-----------------------------------------------------------------------|------|--------------------------------------------------------|
| [**Апрель**](taskschedulerschema-april-monthstype-element.md)         | Недоступно  | Указывает, что задача выполняется в апреле. <br/>     |
| [**Август**](taskschedulerschema-august-monthstype-element.md)       | Недоступно  | Указывает, что задача выполняется в августе. <br/>    |
| [**Декабрь**](taskschedulerschema-december-monthstype-element.md)   | Недоступно  | Указывает, что задача выполняется в декабре. <br/>  |
| [**Февраль**](taskschedulerschema-february-monthstype-element.md)   | Недоступно  | Указывает, что задача выполняется в феврале. <br/>  |
| [**Январь**](taskschedulerschema-january-monthstype-element.md)     | Недоступно  | Указывает, что задача выполняется в январе. <br/>   |
| [**Июль**](taskschedulerschema-july-monthstype-element.md)           | Недоступно  | Указывает, что задача выполняется в июле. <br/>      |
| [**Июнь**](taskschedulerschema-june-monthstype-element.md)           | Недоступно  | Указывает, что задача выполняется в июне. <br/>      |
| [**Март**](taskschedulerschema-march-monthstype-element.md)         | Недоступно  | Указывает, что задача выполняется в марте. <br/>     |
| [**Май**](taskschedulerschema-may-monthstype-element.md)             | Недоступно  | Указывает, что задача выполняется в Май. <br/>       |
| [**Ноябрь**](taskschedulerschema-november-monthstype-element.md)   | Недоступно  | Указывает, что задача выполняется в ноябре. <br/>  |
| [**Октябрь**](taskschedulerschema-october-monthstype-element.md)     | Недоступно  | Указывает, что задача выполняется в октябре. <br/>   |
| [**Сентябрь**](taskschedulerschema-september-monthstype-element.md) | Недоступно  | Указывает, что задача выполняется в сентябре. <br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач сложные типы схемы](task-scheduler-schema-complex-types.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





