---
title: Суббота (Дайсофвиктипе), элемент
description: Указывает, что задача выполняется в субботу.
ms.assetid: def26a72-c143-466a-b5b0-6105078afffa
keywords:
- Элемент субботы планировщик задач
topic_type:
- apiref
api_name:
- Saturday
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1b5f7cb36002b2add64cdea541caa2fd28df37ff
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264968"
---
# <a name="saturday-daysofweektype-element"></a>Суббота (Дайсофвиктипе), элемент

Указывает, что задача выполняется в субботу.

``` syntax
<xs:element name="Saturday">
    <xs:complexType />
</xs:element>
```

Элемент **субботы** определяется сложным типом [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                                                  | Унаследован от                                                             | Описание                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| [**DaysOfWeek (Монслидайофвиксчедулетипе)**](taskschedulerschema-daysofweek-monthlydayofweekscheduletype-element.md) | [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) | Указывает дни недели, в которых задача выполняется для ежемесячного расписания недели.<br/> |
| [**DaysOfWeek (Виклисчедулетипе)**](taskschedulerschema-daysofweek-weeklyscheduletype-element.md)                     | [**дайсофвиктипе**](taskschedulerschema-daysofweektype-complextype.md) | Указывает дни недели, в которых задача выполняется для еженедельного расписания.<br/>              |



## <a name="examples"></a>Примеры

Следующий XML-код определяет календарь дня недели, который запускает задачу в субботу.


```XML
<DaysOfWeek>
    <Saturday/>
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

 

 





