---
title: Буттригжер (Тригжерграуп), элемент
description: Указывает триггер, который запускает задачу при загрузке системы.
ms.assetid: c6833547-0daf-4e8a-b8c5-b422827b1d96
keywords:
- планировщик задач триггера загрузки, XML-элемент
- планировщик задач элемента Буттригжер
topic_type:
- apiref
api_name:
- BootTrigger
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1a9067c5e343db0e3bce0972dc89bfc9fd8857d34a3ff9bd9fd65909c019c2e9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119309574"
---
# <a name="boottrigger-triggergroup-element"></a>Буттригжер (Тригжерграуп), элемент

Указывает триггер, который запускает задачу при загрузке системы.

``` syntax
<xs:element name="BootTrigger"
    type="bootTriggerType"
 />
```

Элемент **буттригжер** определяется сложным типом [**буттригжертипе**](taskschedulerschema-boottriggertype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                           | Унаследован от                                                         | Описание                                            |
|-------------------------------------------------------------------|----------------------------------------------------------------------|--------------------------------------------------------|
| [**Триггеры**](taskschedulerschema-triggers-tasktype-element.md) | [**тригжерстипе**](taskschedulerschema-triggerstype-complextype.md) | Задает триггеры, которые запускают задачу.<br/> |



## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                                        | Тип                                                                     | Описание                                                                                                                        |
|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| [**Задержка (Буттригжертипе)**](taskschedulerschema-delay-boottriggertype-element.md)                           | длительность                                                                 | Указывает промежуток времени между загрузкой системы и началом задачи.<br/>                            |
| [**Включено (Тригжербасетипе)**](taskschedulerschema-enabled-triggerbasetype-element.md)                       | Логическое                                                                  | Указывает, что триггер включен.<br/>                                                                                  |
| [**Ендбаундари (Тригжербасетипе)**](taskschedulerschema-endboundary-triggerbasetype-element.md)               | dateTime                                                                 | Указывает дату и время деактивации триггера. Триггер не может запустить задачу после ее деактивации.<br/> |
| [**Ексекутионтимелимит (Тригжербасетипе)**](taskschedulerschema-executiontimelimit-triggerbasetype-element.md) | длительность                                                                 | Указывает максимальное время, в течение которого задача может запускаться триггером.<br/>                                   |
| [**Повторение (Тригжербасетипе)**](taskschedulerschema-repetition-triggerbasetype-element.md)                 | [**репетитионтипе**](taskschedulerschema-repetitiontype-complextype.md) | Указывает, как часто выполняется задача и как долго шаблон повторения повторяется после запуска задачи.<br/>          |
| [**Стартбаундари (Тригжербасетипе)**](taskschedulerschema-startboundary-triggerbasetype-element.md)           | dateTime                                                                 | Указывает дату и время активации триггера.<br/>                                                              |



## <a name="attributes"></a>Атрибуты



| Имя | Тип       | Описание                               |
|------|------------|-------------------------------------------|
| Идентификатор   | **строка** | Идентификатор триггера.<br/> |



## <a name="remarks"></a>Remarks

Для разработки скриптов триггер загрузки определяется объектом [**буттригжер**](boottrigger.md) .

Для разработки на C++ триггер загрузки определяется объектом [**ибуттригжер**](/windows/desktop/api/taskschd/nn-taskschd-iboottrigger) .

## <a name="examples"></a>Примеры

Полный пример XML-кода для задачи, указывающей триггер загрузки, см. в разделе [Пример загрузочного триггера (XML)](boot-trigger-example--xml-.md).

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

 

 





