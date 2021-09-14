---
title: Элемент Date (Регистратионинфотипе)
description: Указывает дату и время регистрации задачи.
ms.assetid: 0b226786-152d-4231-afa6-db5a630525f3
keywords:
- Элемент Date планировщик задач
topic_type:
- apiref
api_name:
- Date
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1e7d61b9cc637fcc39c8bfd114999a84ede4153d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064498"
---
# <a name="date-registrationinfotype-element"></a>Элемент Date (Регистратионинфотипе)

Указывает дату и время регистрации задачи.

``` syntax
<xs:element name="Date"
    type="dateTime"
    minOccurs="0"
 />
```

Элемент **Date** определяется сложным типом [**регистратионинфотипе**](taskschedulerschema-registrationinfotype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                           | Унаследован от                                                                         | Описание                                                                                                                         |
|-----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| [**регистратионинфо**](taskschedulerschema-registrationinfo-tasktype-element.md) | [**регистратионинфотипе**](taskschedulerschema-registrationinfotype-complextype.md) | Указывает административную информацию о задаче, например автора задачи и дату регистрации задачи.<br/> |



## <a name="remarks"></a>Remarks

Для разработки сценариев Дата регистрации задачи указывается с помощью свойства [**регистратионинфо. Date**](registrationinfo-date.md) .

Для разработки на C++ Дата регистрации задачи указывается с помощью свойства [**ирегистратионинфо::D ATE**](/windows/desktop/api/taskschd/nf-taskschd-iregistrationinfo-get_date) .

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

 

 





