---
title: Сложный тип Тригжерстипе
description: Определяет группу (Тригжерграуп) для всех элементов Trigger.
ms.assetid: ceabc332-e028-491e-8fd8-c02ac23a2635
keywords:
- планировщик задач сложного типа Тригжерстипе
topic_type:
- apiref
api_name:
- triggersType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9903fdc292fe832cc6931d794a4c1f39fd91f83e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968586"
---
# <a name="triggerstype-complex-type"></a>Сложный тип Тригжерстипе

Определяет группу ([**тригжерграуп**](taskschedulerschema-triggergroup-group.md)) для всех элементов Trigger. Группа [**тригжерграуп**](taskschedulerschema-triggergroup-group.md) содержит список триггеров, которые можно использовать в задаче.

``` syntax
<xs:complexType name="triggersType">
    <xs:group
        minOccurs="0"
        maxOccurs="48"
        ref="triggerGroup"
     />
</xs:complexType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





