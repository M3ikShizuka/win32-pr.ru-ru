---
title: Регистратионинфо (taskType), элемент
description: Указывает административную информацию о задаче, например автора задачи и дату регистрации задачи.
ms.assetid: f3961bad-e9a3-4626-87ed-9639d912717d
keywords:
- планировщик задач сведения о регистрации, XML-элемент
- планировщик задач элемента Регистратионинфо
topic_type:
- apiref
api_name:
- RegistrationInfo
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 45b912bc9f870c39cec9ff37df95df46599c0158dd08bf3ca1d47cee29058979
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119059772"
---
# <a name="registrationinfo-tasktype-element"></a>Регистратионинфо (taskType), элемент

Указывает административную информацию о задаче, например автора задачи и дату регистрации задачи.

``` syntax
<xs:element name="RegistrationInfo"
    type="registrationInfoType"
    minOccurs="0"
 />
```

Элемент **регистратионинфо** определяется сложным типом [**TaskType**](taskschedulerschema-tasktype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                          | Унаследован от                                                 | Описание                                                                  |
|--------------------------------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------|
| [**Задача**](taskschedulerschema-task-element.md) | [**taskType**](taskschedulerschema-tasktype-complextype.md) | Определяет задачу, выполняемую службой планировщик задач.<br/> |



## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                                                  | Тип     | Описание                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------|----------|---------------------------------------------------------------------------------------------------------------------------|
| [**Автор (Регистратионинфотипе)**](taskschedulerschema-author-registrationinfotype-element.md)                         | строка   | Указывает автора задачи.<br/>                                                                              |
| [**Дата (Регистратионинфотипе)**](taskschedulerschema-date-registrationinfotype-element.md)                             | dateTime | Указывает дату и время регистрации задачи.<br/>                                                       |
| [**Описание (Регистратионинфотипе)**](taskschedulerschema-description-registrationinfotype-element.md)               | строка   | Указание описания задачи.<br/>                                                                         |
| [**Документация (Регистратионинфотипе)**](taskschedulerschema-documentation-registrationinfotype-element.md)           | строка   | Указывает любую дополнительную документацию для задачи.<br/>                                                           |
| [**SecurityDescriptor (Регистратионинфотипе)**](taskschedulerschema-securitydescriptor-registrationinfotype-element.md) | строка   | Указывает дескриптор безопасности задачи.<br/>                                                                 |
| [**Источник (Регистратионинфотипе)**](taskschedulerschema-source-registrationinfotype-element.md)                         | строка   | Указывает, откуда поступила задача. Например, из компонента, службы, приложения или пользователя.<br/> |
| [**URI (Регистратионинфотипе)**](taskschedulerschema-uri-registrationinfotype-element.md)                               | anyURI   | Указывает универсальный код ресурса (URI) задачи.<br/>                                                                                 |
| [**Версия (Регистратионинфотипе)**](taskschedulerschema-version-registrationinfotype-element.md)                       | строка   | Указывает номер версии задачи.<br/>                                                                      |



## <a name="remarks"></a>Remarks

Для разработки сценариев сведения о регистрации задачи указываются с помощью свойства [**таскдефинитион. регистратионинфо**](taskdefinition-registrationinfo.md) .

Для разработки на C++ сведения о регистрации задачи указываются с помощью [**Свойства регистратионинфо объекта итаскдефинитион**](/windows/desktop/api/taskschd/nf-taskschd-itaskdefinition-get_registrationinfo).

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

 

 





