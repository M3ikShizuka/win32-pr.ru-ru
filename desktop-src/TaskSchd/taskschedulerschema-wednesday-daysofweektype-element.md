---
title: Среда (Дайсофвиктипе), элемент
description: Указывает, что задача выполняется в среду.
ms.assetid: 6d4f52e2-4390-4f9d-bab8-813bd0851582
keywords:
- Элемент среды планировщик задач
topic_type:
- apiref
api_name:
- Wednesday
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3f9d8c60cb7cea818cc0b096e99e97e8f1490d47
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462616"
---
# <a name="wednesday-daysofweektype-element"></a>Среда (Дайсофвиктипе), элемент

Указывает, что задача выполняется в среду.

``` syntax
<xs:element name="Wednesday">
    <xs:complexType />
</xs:element>
```

Элемент **среды** определяется сложным типом [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                                                  | Унаследован от                                                             | Описание                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| [**DaysOfWeek (Монслидайофвиксчедулетипе)**](taskschedulerschema-daysofweek-monthlydayofweekscheduletype-element.md) | [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) | Указывает дни недели, в которых задача выполняется для ежемесячного расписания недели.<br/> |
| [**DaysOfWeek (Виклисчедулетипе)**](taskschedulerschema-daysofweek-weeklyscheduletype-element.md)                     | [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) | Указывает дни недели, в которых задача выполняется для еженедельного расписания.<br/>              |



## <a name="examples"></a>Примеры

Следующий XML-код определяет календарь дня недели, который запускает задачу в среду.


```XML
<DaysOfWeek>
    <Wednesday/>
</DaysOfWeek>
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

 

 





