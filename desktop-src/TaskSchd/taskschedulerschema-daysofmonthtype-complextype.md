---
title: Сложный тип Дайсофмонстипе
description: Определяет дочерний элемент и сведения о последовательности для элемента DaysOfMonth (Монслисчедулетипе).
ms.assetid: 8258c090-c836-497e-8e5b-db4782277822
keywords:
- планировщик задач сложного типа Дайсофмонстипе
topic_type:
- apiref
api_name:
- daysOfMonthType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a32f2d0b3084e5146e53370d1771018a5d27a025f5ea419a61d8c39804d5611a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120010854"
---
# <a name="daysofmonthtype-complex-type"></a>Сложный тип Дайсофмонстипе

Определяет дочерний элемент и сведения о последовательности для элемента [**DaysOfMonth (монслисчедулетипе)**](taskschedulerschema-daysofmonth-monthlyscheduletype-element.md) .

``` syntax
<xs:complexType name="daysOfMonthType">
    <xs:sequence>
        <xs:element name="Day"
            type="dayOfMonthType"
            minOccurs="0"
            maxOccurs="32"
         />
    </xs:sequence>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                        | Тип                                                                    | Описание                                                          |
|----------------------------------------------------------------|-------------------------------------------------------------------------|----------------------------------------------------------------------|
| [**День**](taskschedulerschema-day-daysofmonthtype-element.md) | [**дайофмонстипе**](taskschedulerschema-dayofmonthtype-simpletype.md) | Указывает день месяца, в который выполняется задача. <br/> |



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

 

 





