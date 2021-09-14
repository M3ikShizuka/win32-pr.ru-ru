---
title: Виксинтервал (Виклисчедулетипе), элемент
description: Указывает интервал между неделями в расписании.
ms.assetid: 6cbf1e7e-a695-4012-97fd-fe3360c362c4
keywords:
- планировщик задач элемента Виксинтервал
topic_type:
- apiref
api_name:
- WeeksInterval
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 747ca4b73ff18bdb3e29d8b909d72b8d2367d89b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374753"
---
# <a name="weeksinterval-weeklyscheduletype-element"></a>Виксинтервал (Виклисчедулетипе), элемент

Указывает интервал между неделями в расписании.

``` syntax
<xs:element name="WeeksInterval"
    minOccurs="0"
>
    <xs:simpleType>
        <xs:restriction
            base="unsignedByte"
        >
            <xs:minInclusive
                value="1"
             />
            <xs:maxInclusive
                value="52"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент определяется сложным типом [**виклисчедулетипе**](taskschedulerschema-weeklyscheduletype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                  | Унаследован от                                                                     | Описание                             |
|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-----------------------------------------|
| [**счедулебивик**](taskschedulerschema-schedulebyweek-calendartriggertype-element.md) | [**виклисчедулетипе**](taskschedulerschema-weeklyscheduletype-complextype.md) | Указывает еженедельное расписание.<br/> |



## <a name="remarks"></a>Remarks

Для разработки сценариев еженедельный интервал указывается с помощью свойства [**виклитригжер. виксинтервал**](weeklytrigger-weeksinterval.md) .

Для разработки на C++ еженедельный интервал задается с помощью свойства [**ивиклитригжер:: виксинтервал**](/windows/desktop/api/taskschd/nf-taskschd-iweeklytrigger-get_weeksinterval) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет еженедельный календарный триггер, который запускает задачу с понедельника по пятницу (в 8:00 AM) каждую неделю.


```XML
<CalendarTrigger>
    <StartBoundary>2005-01-01T08:00:00</StartBoundary>
    <EndBounadry>2007-01-01T00:00:00</EndBoundary>
    <ScheduleByWeek>
        <WeeksInterval>1</WeeksInterval>
        <DaysOfWeek>
            <Monday/>
            <Tuesday/>
            <Wednesday/>
            <Thurday/>
            <Friday/>
        </DaysOfWeek>
    </ScheduleByWeek>
</CalendarTrigger>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





