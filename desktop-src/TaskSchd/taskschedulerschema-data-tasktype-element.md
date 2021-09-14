---
title: Элемент Data (taskType)
description: Определяет дополнительные данные, связанные с задачей, но в противном случае не используется службой планировщик задач.
ms.assetid: 296cd33d-5f82-4de7-84a7-e791619ad0b5
keywords:
- Элемент данных планировщик задач
topic_type:
- apiref
api_name:
- Data
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3afff1cbd81ede49568afdc9e516d87a57ff9e5a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064502"
---
# <a name="data-tasktype-element"></a>Элемент Data (taskType)

Определяет дополнительные данные, связанные с задачей, но в противном случае не используется службой планировщик задач.

``` syntax
<xs:element name="Data"
    type="dataType"
 />
```

Элемент **Data** определяется сложным типом [**TaskType**](taskschedulerschema-tasktype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                          | Унаследован от                                                 | Описание                                                                  |
|--------------------------------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------|
| [**Задача**](taskschedulerschema-task-element.md) | [**taskType**](taskschedulerschema-tasktype-complextype.md) | Определяет задачу, выполняемую службой планировщик задач.<br/> |



## <a name="remarks"></a>Remarks

В качестве примера данных этого типа служба журналы и оповещения производительности использует это свойство в качестве контейнера хранилища для запроса счетчика производительности, связанного с задачей.

Для разработки на C++ данные задачи указываются с помощью [**свойства Data объекта итаскдефинитион**](/windows/desktop/api/taskschd/nf-taskschd-itaskdefinition-get_data).

При разработке сценариев данные задачи указываются с помощью свойства [**таскдефинитион. Data**](taskdefinition-data.md) .

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

 

 





