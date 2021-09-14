---
title: Объект ActionCollection
description: Объект скрипта, содержащий действия, выполняемые задачей.
ms.assetid: e887680d-e7e8-4bea-8f00-fb7645d79e60
keywords:
- действия планировщик задач, объект Collection
- планировщик задач объекта ActionCollection
- Планировщик задач объекта ActionCollection, описание
topic_type:
- apiref
api_name:
- ActionCollection
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 89dee7182cc79684dec1fd052f7ad67409ba513f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056643"
---
# <a name="actioncollection-object"></a>Объект ActionCollection

Объект скрипта, содержащий действия, выполняемые задачей.

## <a name="members"></a>Элементы

Объект **ActionCollection** имеет следующие типы членов:

-   [Методы](#methods)
-   [Свойства](#properties)

### <a name="methods"></a>Методы

Объект **ActionCollection** содержит эти методы.



| Метод                                    | Описание                                                 |
|:------------------------------------------|:------------------------------------------------------------|
| [**Открытым**](actioncollection-clear.md)   | Удаляет все действия из коллекции.<br/>      |
| [**Создание**](actioncollection-create.md) | Создает и добавляет новое действие в коллекцию.<br/> |
| [**Удалить**](actioncollection-remove.md) | Удаляет указанное действие из коллекции.<br/>  |



 

### <a name="properties"></a>Свойства

Объект **ActionCollection** имеет следующие свойства.



| Свойство                                               | Тип доступа           | Описание                                                           |
|:-------------------------------------------------------|:----------------------|:----------------------------------------------------------------------|
| [**Контекст**](actioncollection-context.md)<br/> | Чтение/запись<br/> | Возвращает или задает идентификатор участника для задачи.<br/> |
| [**Расчета**](actioncollection-count.md)<br/>     | Только для чтения<br/>  | Возвращает количество действий в коллекции.<br/>              |
| [**Элемент**](actioncollection-item.md)<br/>       | Только для чтения<br/>  | Возвращает указанное действие из коллекции.<br/>               |
| [**XmlText**](actioncollection-xmltext.md)<br/> | Чтение/запись<br/> | Возвращает или задает версию коллекции в формате XML.<br/>   |



 

## <a name="remarks"></a>Комментарии

При чтении или записи XML действия задачи указываются в элементе [**Actions**](taskschedulerschema-actions-tasktype-element.md) схемы планировщик задач.

## <a name="examples"></a>Примеры

Дополнительные сведения и примеры кода для этого объекта скрипта см. в разделе [пример триггера времени (сценарии](time-trigger-example--scripting-.md)), пример триггера [события (](https://www.bing.com/search?q=Event+Trigger+Example+(Scripting))сценарии) [, пример ежедневного триггера](daily-trigger-example--scripting-.md)(сценарии), пример триггера [регистрации](registration-trigger-example--scripting-.md)(сценарии) [, пример](weekly-trigger-example--scripting-.md)триггера [входа](logon-trigger-example--scripting-.md)(скрипт), пример триггера [загрузки](boot-trigger-example--scripting-.md)(скрипт).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



 

 





