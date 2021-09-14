---
title: Усеунифиедсчедулинженгине (Сеттингстипе), элемент
description: Указывает, что для выполнения этой задачи будет использоваться единый механизм планирования.
ms.assetid: 93436f14-1caf-4ec8-bf74-a198b7dcb27c
keywords:
- планировщик задач элемента Усеунифиедсчедулинженгине
topic_type:
- apiref
api_name:
- UseUnifiedSchedulingEngine
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a00798a46df3dfbb351dd8705b264192c38daff6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968569"
---
# <a name="useunifiedschedulingengine-settingstype-element"></a>Усеунифиедсчедулинженгине (Сеттингстипе), элемент

Указывает, что для выполнения этой задачи будет использоваться единый механизм планирования.

``` syntax
<xs:element name="UseUnifiedSchedulingEngine"
    type="boolean"
    default="false"
    minOccurs="0"
 />
```

Элемент **усеунифиедсчедулинженгине** определяется сложным типом [**сеттингстипе**](taskschedulerschema-settingstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                           | Унаследован от                                                         | Описание                                                                        |
|-------------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------------------------------------------------|
| [**Параметры**](taskschedulerschema-settings-tasktype-element.md) | [**сеттингстипе**](taskschedulerschema-settingstype-complextype.md) | Содержит параметры, которые планировщик задач использует для выполнения задачи.<br/> |



## <a name="remarks"></a>Комментарии

Значение по умолчанию для этого элемента — false.

Для разработки на C++ эта информация доступна через свойство [**ITaskSettings2:: усеунифиедсчедулинженгине**](/windows/desktop/api/taskschd/nf-taskschd-itasksettings2-get_useunifiedschedulingengine) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет элемент Settings, который указывает, что для выполнения этой задачи будет использоваться единый механизм планирования.


```XML
<Settings>
    <UseUnifiedSchedulingEngine>true</UseUnifiedSchedulingEngine>
</Settings>
        
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





