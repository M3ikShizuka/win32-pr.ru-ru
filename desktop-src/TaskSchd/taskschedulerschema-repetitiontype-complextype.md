---
title: Сложный тип Репетитионтипе
description: Определяет дочерние элементы и сведения о последовательности для элемента повторения (Тригжербасетипе).
ms.assetid: d2b4b840-3a69-4ff8-ac32-6ec76e7e8788
keywords:
- планировщик задач сложного типа Репетитионтипе
topic_type:
- apiref
api_name:
- repetitionType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3d45f83be8ab8b37211224ec9f284a71cdde6bfc06032c5d05df9e5dee8bf4ae
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119772094"
---
# <a name="repetitiontype-complex-type"></a>Сложный тип Репетитионтипе

Определяет дочерние элементы и сведения о последовательности для элемента [**повторения (тригжербасетипе)**](taskschedulerschema-repetition-triggerbasetype-element.md) .

``` syntax
<xs:complexType name="repetitionType">
    <xs:all>
        <xs:element name="Interval">
            <xs:simpleType>
                <xs:restriction
                    base="duration"
                >
                    <xs:minInclusive
                        value="PT1M"
                     />
                    <xs:maxInclusive
                        value="P31D"
                     />
                </xs:restriction>
            </xs:simpleType>
        </xs:element>
        <xs:element name="Duration"
            minOccurs="0"
        >
            <xs:simpleType>
                <xs:restriction
                    base="duration"
                >
                    <xs:minInclusive
                        value="PT1M"
                     />
                </xs:restriction>
            </xs:simpleType>
        </xs:element>
        <xs:element name="StopAtDurationEnd"
            type="boolean"
            default="false"
            minOccurs="0"
         />
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                   | Тип    | Описание                                                                                                            |
|-------------------------------------------------------------------------------------------|---------|------------------------------------------------------------------------------------------------------------------------|
| [**Длительность**](taskschedulerschema-duration-repetitiontype-element.md)                   |         | Указывает, как долго шаблон повторяется. Если значение не указано, шаблон повторяется бесконечно.<br/> |
| [**Интервал**](taskschedulerschema-interval-repetitiontype-element.md)                   |         | Задает интервал времени между перезапусками задачи.<br/>                                              |
| [**стопатдуратионенд**](taskschedulerschema-stopatdurationend-repetitiontype-element.md) | Логическое | Указывает, что выполняющийся экземпляр задачи останавливается в конце срока действия шаблона повторения.<br/>     |



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

 

 





