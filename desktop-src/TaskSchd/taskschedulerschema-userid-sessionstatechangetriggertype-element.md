---
title: UserId (Сессионстатечанжетригжертипе), элемент
description: Содержит пользователя для сеанса сервера терминалов. При обнаружении изменения состояния сеанса для этого пользователя запускается задача.
ms.assetid: 7605f444-b2c9-4bba-a035-f1307c01184f
keywords:
- Элемент UserId планировщик задач
topic_type:
- apiref
api_name:
- UserId
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: cd66a05d25ea9b44f124d55ccc0cbb2c628aeeb5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968562"
---
# <a name="userid-sessionstatechangetriggertype-element"></a>UserId (Сессионстатечанжетригжертипе), элемент

Содержит пользователя для сеанса сервера терминалов. При обнаружении изменения состояния сеанса для этого пользователя запускается задача.

``` syntax
<xs:element name="UserId"
    type="nonEmptyString"
    maxOccurs="1"
    minOccurs="0"
 />
```

Элемент **UserID** определяется сложным типом [**сессионстатечанжетригжертипе**](taskschedulerschema-sessionstatechangetriggertype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                       | Унаследован от                                                                                           | Описание                                                                                     |
|-------------------------------|--------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **сессионстатечанжетригжер** | [**сессионстатечанжетригжертипе**](taskschedulerschema-sessionstatechangetriggertype-complextype.md) | Указывает триггер, который запускает задачу при изменении состояния сеанса сервера терминалов.<br/> |



## <a name="remarks"></a>Комментарии

Сведения о разработке на языке C++ см. в разделе [**свойство UserId объекта исессионстатечанжетригжер**](/windows/desktop/api/taskschd/nf-taskschd-isessionstatechangetrigger-get_userid).

Сведения о разработке сценариев см. в разделе [**сессионстатечанжетригжер. UserID**](sessionstatechangetrigger-userid.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





