---
title: Элемент Data (Комхандлертипе)
description: Указывает дополнительные данные, связанные с обработчиком.
ms.assetid: 352cb92b-54bb-4bb0-8a43-123c88c80962
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
ms.openlocfilehash: d009005dc2bb889c8bd9e34e84d853665310330a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064503"
---
# <a name="data-comhandlertype-element"></a>Элемент Data (Комхандлертипе)

Указывает дополнительные данные, связанные с обработчиком.

``` syntax
<xs:element name="Data"
    type="dataType"
 />
```

Элемент **Data** определяется сложным типом [**комхандлертипе**](taskschedulerschema-comhandlertype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                  | Унаследован от                                                             | Описание                                          |
|--------------------------------------------------------------------------|--------------------------------------------------------------------------|------------------------------------------------------|
| [**комхандлер**](taskschedulerschema-comhandler-actiongroup-element.md) | [**комхандлертипе**](taskschedulerschema-comhandlertype-complextype.md) | Указывает действие, которое вызывает обработчик.<br/> |



## <a name="remarks"></a>Remarks

Приложения определяют данные обработчика с помощью свойства [**Data**](/windows/desktop/api/taskschd/nf-taskschd-icomhandleraction-get_data) интерфейса [**икомхандлерактион**](/windows/desktop/api/taskschd/nn-taskschd-icomhandleraction) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





