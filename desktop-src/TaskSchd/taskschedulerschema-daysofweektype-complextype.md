---
title: Сложный тип Дайсофвиктипе
description: Определяет дочерние элементы и сведения о последовательности для элементов DaysOfWeek (Виклисчедулетипе) и DaysOfWeek (Монслидайофвиксчедулетипе).
ms.assetid: b3315582-af7a-4d4c-8f6f-61de12a85f46
keywords:
- планировщик задач сложного типа Дайсофвиктипе
topic_type:
- apiref
api_name:
- daysOfWeekType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 0b4a1b5e6aeaa77c0bdfe12b1d5b68fde018f236
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066882"
---
# <a name="daysofweektype-complex-type"></a>Сложный тип Дайсофвиктипе

Определяет дочерние элементы и сведения о последовательности для элементов [**DaysOfWeek (виклисчедулетипе)**](taskschedulerschema-daysofweek-weeklyscheduletype-element.md) и [**DaysOfWeek (монслидайофвиксчедулетипе)**](taskschedulerschema-daysofweek-monthlydayofweekscheduletype-element.md) .

``` syntax
<xs:complexType name="daysOfWeekType">
    <xs:all>
        <xs:element name="Monday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Tuesday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Wednesday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Thursday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Friday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Saturday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
        <xs:element name="Sunday"
            minOccurs="0"
        >
            <xs:complexType />
        </xs:element>
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                   | Тип | Описание                         |
|---------------------------------------------------------------------------|------|-------------------------------------|
| [**Пятница**](taskschedulerschema-friday-daysofweektype-element.md)       | Недоступно  | Задача выполняется в пятницу. <br/>    |
| [**Понедельник**](taskschedulerschema-monday-daysofweektype-element.md)       | Недоступно  | Задача выполняется в понедельник.<br/>     |
| [**Сегодня**](taskschedulerschema-saturday-daysofweektype-element.md)   | Недоступно  | Задача выполняется в субботу. <br/>  |
| [**Воскресенье**](taskschedulerschema-sunday-daysofweektype-element.md)       | Недоступно  | Задача выполняется в воскресенье. <br/>    |
| [**Четверг**](taskschedulerschema-thursday-daysofweektype-element.md)   | Недоступно  | Задача выполняется в четверг <br/>   |
| [**Вторник**](taskschedulerschema-tuesday-daysofweektype-element.md)     | Недоступно  | Задача выполняется во вторник. <br/>   |
| [**Среда**](taskschedulerschema-wednesday-daysofweektype-element.md) | Недоступно  | Задача выполняется в среду. <br/> |



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

 

 





