---
title: Сложный тип Логонтригжертипе
description: Определяет дочерние элементы и сведения о последовательности для элемента Логонтригжер.
ms.assetid: ddb1d01b-89d1-4d52-872c-4fbd90f32f4b
keywords:
- планировщик задач сложного типа Логонтригжертипе
topic_type:
- apiref
api_name:
- logonTriggerType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 81a3f42eb94d14506d96348b803c8b1bc41737d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259184"
---
# <a name="logontriggertype-complex-type"></a>Сложный тип Логонтригжертипе

Определяет дочерние элементы и сведения о последовательности для элемента [**логонтригжер**](taskschedulerschema-logontrigger-triggergroup-element.md) .

``` syntax
<xs:complexType name="logonTriggerType">
    <xs:complexContent>
        <xs:extension
            base="triggerBaseType"
        >
            <xs:sequence>
                <xs:element name="UserId"
                    type="nonEmptyString"
                    minOccurs="0"
                 />
                <xs:element name="Delay"
                    type="duration"
                    default="PT0M"
                    minOccurs="0"
                 />
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                               | Тип                                                                    | Описание                                                                                   |
|-----------------------------------------------------------------------|-------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [**Задержка**](taskschedulerschema-delay-logontriggertype-element.md)   | длительность                                                                | Промежуток времени между входом пользователя в систему и запуском задачи.<br/>         |
| [**UserId**](taskschedulerschema-userid-logontriggertype-element.md) | [**нонемптистринг**](taskschedulerschema-nonemptystring-simpletype.md) | Идентификатор пользователя. Задача запускается, когда пользователь входит в систему на компьютере.<br/> |



## <a name="remarks"></a>Remarks

Помимо дочерних элементов, определенных здесь, элемент [**логонтригжер**](taskschedulerschema-logontrigger-triggergroup-element.md) также использует дочерние элементы, определенные сложным типом [**тригжербасетипе**](taskschedulerschema-triggerbasetype-complextype.md) .

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

 

 





