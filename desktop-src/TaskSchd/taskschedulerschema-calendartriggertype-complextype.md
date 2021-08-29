---
title: Сложный тип Календартригжертипе
description: Определяет дочерние элементы и сведения о последовательности для элементов календаря.
ms.assetid: bf0d964e-aff2-4807-b086-c504f8963663
keywords:
- планировщик задач сложного типа Календартригжертипе
topic_type:
- apiref
api_name:
- calendarTriggerType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 62b6aa2c3c1aff0e6e9cb706ede58c1b21af79fb7a5bae812a992e68bbd28b7f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119866654"
---
# <a name="calendartriggertype-complex-type"></a>Сложный тип Календартригжертипе

Определяет дочерние элементы и сведения о последовательности для элементов календаря.

``` syntax
<xs:complexType name="calendarTriggerType">
    <xs:complexContent>
        <xs:extension
            base="triggerBaseType"
        >
            <xs:sequence>
                <xs:element name="RandomDelay"
                    type="duration"
                    default="PT0M"
                    minOccurs="0"
                 />
                <xs:choice>
                    <xs:element name="ScheduleByDay"
                        type="dailyScheduleType"
                     />
                    <xs:element name="ScheduleByWeek"
                        type="weeklyScheduleType"
                     />
                    <xs:element name="ScheduleByMonth"
                        type="monthlyScheduleType"
                     />
                    <xs:element name="ScheduleByMonthDayOfWeek"
                        type="monthlyDayOfWeekScheduleType"
                     />
                </xs:choice>
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                                      | Тип                                                                                                 | Описание                                                                                                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**рандомделай**](taskschedulerschema-randomdelay-calendartriggertype-element.md)                           | длительность                                                                                             | Содержит время задержки, которое случайным образом добавляется к времени начала триггера. Формат этой строки — `P<days>DT<hours>H<minutes>M<seconds>S` (например, P2DT5S имеет 2 дня, 5 секунд задержки).<br/> |
| [**счедулебидай**](taskschedulerschema-schedulebyday-calendartriggertype-element.md)                       | [**даилисчедулетипе**](taskschedulerschema-dailyscheduletype-complextype.md)                       | Указывает ежедневное расписание. Например, задача запускается каждый день, каждый второй день, каждый третий день и т. д.<br/>                                                                                                               |
| [**счедулебимонс**](taskschedulerschema-schedulebymonth-calendartriggertype-element.md)                   | [**монслисчедулетипе**](taskschedulerschema-monthlyscheduletype-complextype.md)                   | Указывает ежемесячное расписание. Например, задача начинается в 8:00 в определенные дни месяца в определенные месяцы. <br/>                                                                                                       |
| [**счедулебимонсдайофвик**](taskschedulerschema-schedulebymonthdayofweek-calendartriggertype-element.md) | [**монслидайофвиксчедулетипе**](taskschedulerschema-monthlydayofweekscheduletype-complextype.md) | Указывает триггер, который запускает задание в месячном расписании недели. Например, задача запускается в определенные дни недели, недели месяца и месяцы года. <br/>                                               |
| [**счедулебивик**](taskschedulerschema-schedulebyweek-calendartriggertype-element.md)                     | [**виклисчедулетипе**](taskschedulerschema-weeklyscheduletype-complextype.md)                     | Указывает еженедельное расписание. Например, задача начинается в 8:00 в конкретный день недели или в конкретный день недели, каждую неделю. <br/>                                                              |



## <a name="remarks"></a>Remarks

Помимо дочернего элемента, определенного здесь, элемент [**календартригжер**](taskschedulerschema-calendartrigger-triggergroup-element.md) также использует дочерние элементы, определенные сложным типом [**тригжербасетипе**](taskschedulerschema-triggerbasetype-complextype.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[планировщик задач сложные типы схемы](task-scheduler-schema-complex-types.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





