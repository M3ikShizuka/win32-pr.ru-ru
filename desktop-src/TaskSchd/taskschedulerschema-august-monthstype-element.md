---
title: Элемент августе (Монсстипе)
description: Указывает, что задача выполняется в августе.
ms.assetid: cd7e528c-d482-4bb4-a31f-fccdb19a441b
keywords:
- планировщик задач элемента августе
topic_type:
- apiref
api_name:
- August
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 8c5a8d4adb6e0bdb855499abef9fbfda1ebe7de2cdcaba21ebde9647352ff57a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119991454"
---
# <a name="august-monthstype-element"></a>Элемент августе (Монсстипе)

Указывает, что задача выполняется в августе.

``` syntax
<xs:element name="August">
    <xs:complexType />
</xs:element>
```

Элемент **августе** определяется сложным типом [**монсстипе**](taskschedulerschema-monthstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                                          | Унаследован от                                                     | Описание                                                                                                |
|------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| [**Месяцы (Монслидайофвиксчедулетипе)**](taskschedulerschema-months-monthlydayofweekscheduletype-element.md) | [**монсстипе**](taskschedulerschema-monthstype-complextype.md) | Указывает месяцы года, в течение которых задача выполняется для ежемесячного расписания недели.<br/> |
| [**Месяцы (Монслисчедулетипе)**](taskschedulerschema-months-monthlyscheduletype-element.md)                   | [**монсстипе**](taskschedulerschema-monthstype-complextype.md) | Указывает месяцы года, в течение которых задача выполняется для ежемесячного расписания.<br/>             |



## <a name="examples"></a>Примеры

Следующий XML-код определяет календарь месяцев, в котором выполняется задача в августе.


```XML
<Months>
    <August/>
</Months>
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

 

 





