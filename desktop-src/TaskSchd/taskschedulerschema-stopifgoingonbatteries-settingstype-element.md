---
title: Стопифгоингонбаттериес (Сеттингстипе), элемент
description: Указывает, что задача будет остановлена при переходе компьютера на питание.
ms.assetid: 0d772dbb-a552-45ed-9dc0-7159f6ef12ed
keywords:
- планировщик задач элемента Стопифгоингонбаттериес
topic_type:
- apiref
api_name:
- StopIfGoingOnBatteries
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 2e7de57cde928760c15dd671010880e824c8979f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968645"
---
# <a name="stopifgoingonbatteries-settingstype-element"></a>Стопифгоингонбаттериес (Сеттингстипе), элемент

Указывает, что задача будет остановлена при переходе компьютера на питание.

``` syntax
<xs:element name="StopIfGoingOnBatteries"
    type="boolean"
    default="true"
    minOccurs="0"
 />
```

Элемент **стопифгоингонбаттериес** определяется сложным типом [**сеттингстипе**](taskschedulerschema-settingstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                           | Унаследован от                                                         | Описание                                                                        |
|-------------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------------------------------------------------|
| [**Параметры**](taskschedulerschema-settings-tasktype-element.md) | [**сеттингстипе**](taskschedulerschema-settingstype-complextype.md) | Содержит параметры, которые планировщик задач использует для выполнения задачи.<br/> |



## <a name="remarks"></a>Комментарии

Значение по умолчанию для этого элемента — false. Обратите внимание, что значение по умолчанию изменилось по сравнению с предыдущими версиями планировщик задач.

Для разработки сценариев этот параметр указывается с помощью свойства [**тасксеттингс. стопифгоингонбаттериес**](tasksettings-stopifgoingonbatteries.md) .

Для разработки на C++ этот параметр указывается с помощью свойства [**итасксеттингс:: стопифгоингонбаттериес**](/windows/desktop/api/taskschd/nf-taskschd-itasksettings-get_stopifgoingonbatteries) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет элемент Settings, который разрешает жесткое завершение задачи.


```XML
<Settings>
    <StopIfGoingOnBatteries>true</StopIfGoingOnBatteries>
</Settings>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





