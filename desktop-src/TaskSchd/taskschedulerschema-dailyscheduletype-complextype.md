---
title: Сложный тип Даилисчедулетипе
description: Определяет дочерние элементы и сведения о последовательности для элемента Счедулебидай.
ms.assetid: e0b1b09f-d72a-4a85-9059-4a917bc0104a
keywords:
- планировщик задач сложного типа Даилисчедулетипе
topic_type:
- apiref
api_name:
- dailyScheduleType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 5982ab7e72a79dc909a4e91fafe363ca4703639d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064507"
---
# <a name="dailyscheduletype-complex-type"></a>Сложный тип Даилисчедулетипе

Определяет дочерние элементы и сведения о последовательности для элемента [**счедулебидай**](taskschedulerschema-schedulebyday-calendartriggertype-element.md) .

``` syntax
<xs:complexType name="dailyScheduleType">
    <xs:all>
        <xs:element name="DaysInterval"
            minOccurs="0"
        >
            <xs:simpleType>
                <xs:restriction
                    base="unsignedInt"
                >
                    <xs:minInclusive
                        value="1"
                     />
                    <xs:maxInclusive
                        value="365"
                     />
                </xs:restriction>
            </xs:simpleType>
        </xs:element>
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                            | Тип | Описание                                                          |
|------------------------------------------------------------------------------------|------|----------------------------------------------------------------------|
| [**дайсинтервал**](taskschedulerschema-daysinterval-dailyscheduletype-element.md) |      | Указывает интервал между днями в расписании. <br/> |



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

 

 





