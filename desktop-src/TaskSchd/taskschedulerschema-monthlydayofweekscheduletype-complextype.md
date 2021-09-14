---
title: Сложный тип Монслидайофвиксчедулетипе
description: Определяет дочерние элементы и сведения о последовательности для элемента Счедулебимонсдайофвик.
ms.assetid: fb4e5ba3-592b-47a4-bedf-5181d2b7a50f
keywords:
- планировщик задач сложного типа Монслидайофвиксчедулетипе
topic_type:
- apiref
api_name:
- monthlyDayOfWeekScheduleType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 782715aed5cbf59a98e996bfa18fdd7c1022227a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259144"
---
# <a name="monthlydayofweekscheduletype-complex-type"></a>Сложный тип Монслидайофвиксчедулетипе

Определяет дочерние элементы и сведения о последовательности для элемента [**счедулебимонсдайофвик**](taskschedulerschema-schedulebymonthdayofweek-calendartriggertype-element.md) .

``` syntax
<xs:complexType name="monthlyDayOfWeekScheduleType">
    <xs:all>
        <xs:element name="Weeks"
            type="weeksType"
            minOccurs="0"
         />
        <xs:element name="DaysOfWeek"
            type="daysOfWeekType"
         />
        <xs:element name="Months"
            type="monthsType"
            minOccurs="0"
         />
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                   | Тип                                                                     | Описание                                                             |
|-------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|
| [**DaysOfWeek**](taskschedulerschema-daysofweek-monthlydayofweekscheduletype-element.md) | [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) | Указывает дни недели, в которые выполняется задача.<br/>   |
| [**Месяц**](taskschedulerschema-months-monthlydayofweekscheduletype-element.md)         | [**монсстипе**](taskschedulerschema-monthstype-complextype.md)         | Указывает месяцы года, в течение которых выполняется задача.<br/> |
| [**Недели**](taskschedulerschema-weeks-monthlydayofweekscheduletype-element.md)           | [**викстипе**](taskschedulerschema-weekstype-complextype.md)           | Указывает недели месяца, в течение которых выполняется задача.<br/> |



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

 

 





