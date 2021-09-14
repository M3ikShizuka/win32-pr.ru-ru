---
title: Элемент Март (Монсстипе)
description: Указывает, что задача выполняется в марте.
ms.assetid: 0cd82405-8e17-483d-88ba-32cae590f6b3
keywords:
- Элемент марта планировщик задач
topic_type:
- apiref
api_name:
- March
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: bf6792cf65ab3aecb74bff82282daa0d8fb2bdc6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259163"
---
# <a name="march-monthstype-element"></a>Элемент Март (Монсстипе)

Указывает, что задача выполняется в марте.

``` syntax
<xs:element name="March">
    <xs:complexType />
</xs:element>
```

Элемент **Март** определяется сложным типом [**монсстипе**](taskschedulerschema-monthstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                                          | Унаследован от                                                     | Описание                                                                                                |
|------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| [**Месяцы (Монслидайофвиксчедулетипе)**](taskschedulerschema-months-monthlydayofweekscheduletype-element.md) | [**монсстипе**](taskschedulerschema-monthstype-complextype.md) | Указывает месяцы года, в течение которых задача выполняется для ежемесячного расписания недели.<br/> |
| [**Месяцы (Монслисчедулетипе)**](taskschedulerschema-months-monthlyscheduletype-element.md)                   | [**монсстипе**](taskschedulerschema-monthstype-complextype.md) | Указывает месяцы года, в течение которых задача выполняется для ежемесячного расписания.<br/>             |



## <a name="examples"></a>Примеры

Следующий XML-код определяет календарь месяцев, который запускает задачу в марте.


```XML
<Months>
    <March/>
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

 

 





