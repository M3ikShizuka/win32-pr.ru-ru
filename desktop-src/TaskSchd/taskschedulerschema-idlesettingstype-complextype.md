---
title: Сложный тип Идлесеттингстипе
description: Определяет дочерние элементы и сведения о последовательности для элемента Идлесеттингс (Сеттингстипе).
ms.assetid: 0f50c4d6-fda9-42cc-8dab-4c9439fbea4b
keywords:
- планировщик задач сложного типа Идлесеттингстипе
topic_type:
- apiref
api_name:
- idleSettingsType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: c11c49266b208f92e52f7c1fc97291af6f99fb59367a389476768e65e99b53c4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119796524"
---
# <a name="idlesettingstype-complex-type"></a>Сложный тип Идлесеттингстипе

Определяет дочерние элементы и сведения о последовательности для элемента [**идлесеттингс (сеттингстипе)**](taskschedulerschema-idlesettings-settingstype-element.md) .

``` syntax
<xs:complexType name="idleSettingsType">
    <xs:all>
        <xs:element name="Duration"
            default="PT10M"
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
        <xs:element name="WaitTimeout"
            default="PT1H"
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
        <xs:element name="StopOnIdleEnd"
            type="boolean"
            default="true"
            minOccurs="0"
         />
        <xs:element name="RestartOnIdle"
            type="boolean"
            default="false"
            minOccurs="0"
         />
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                  | Тип    | Описание                                                                                                                                                                                                       |
|------------------------------------------------------------------------------------------|---------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Длительность**](taskschedulerschema-duration-idlesettingstype-element.md)                |         | Указывает время, отведенное на запуск задачи в условиях простоя.<br/>                                                                                                                     |
| [**рестартонидле**](taskschedulerschema-restartonidle-idlesettingstype-element.md)      | Логическое | Задача перезапускается сразу же после запуска условия простоя.<br/>                                                                                                                                             |
| [**стопонидлинд**](taskschedulerschema-terminateonidleend-idlesettingstype-element.md) | Логическое | Указывает, что задача завершается, если условие простоя заканчивается до превышения длительности простоя.<br/>                                                                                                 |
| [**ваиттимеаут**](taskschedulerschema-waittimeout-idlesettingstype-element.md)          |         | Указывает период времени, в течение которого ожидается запуск условия простоя. Если для этого элемента не указано значение, то служба планировщик задач будет ждать неопределенное время, пока не произойдет условие простоя.<br/> |



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

 

 





