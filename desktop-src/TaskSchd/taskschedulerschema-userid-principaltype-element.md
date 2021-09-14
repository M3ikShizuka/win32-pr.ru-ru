---
title: UserId (ПринЦипалтипе), элемент
description: Указывает идентификатор пользователя, необходимый для выполнения задач, связанных с участником.
ms.assetid: 7f3c92bf-c982-4155-9391-862f674a3665
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
ms.openlocfilehash: fe12f76c35238251e2ecc60f848e2f7eb4eaa681
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968565"
---
# <a name="userid-principaltype-element"></a>UserId (ПринЦипалтипе), элемент

Указывает идентификатор пользователя, необходимый для выполнения задач, связанных с участником.

``` syntax
<xs:element name="UserId"
    type="nonEmptyString"
 />
```

Элемент **UserID** определяется сложным типом [**принЦипалтипе**](taskschedulerschema-principaltype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                  | Унаследован от                                                           | Описание                                                    |
|--------------------------------------------------------------------------|------------------------------------------------------------------------|----------------------------------------------------------------|
| [**Основного**](taskschedulerschema-principal-principaltype-element.md) | [**principalType**](taskschedulerschema-principaltype-complextype.md) | Указывает учетные данные безопасности для участника.<br/> |



## <a name="remarks"></a>Комментарии

Элемент **UserID** и элемент [**LogonType**](taskschedulerschema-logontype-principaltype-element.md) используются вместе для определения пользователя, необходимого для выполнения этих задач, использующих этот участник.

Нельзя одновременно указать идентификатор пользователя и идентификатор группы. Укажите либо **идентификатор UserID** , либо элемент [**groupId**](taskschedulerschema-groupid-principaltype-element.md) , но не оба.

Для разработки сценариев идентификатор пользователя указывается с помощью свойства [**Principal. UserID**](principal-userid.md) .

Для разработки на C++ идентификатор пользователя указывается с помощью свойства [**IPrincipal:: UserID**](/windows/desktop/api/taskschd/nf-taskschd-iprincipal-get_userid) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет принцип, используя идентификатор пользователя.


```XML
<Principal>
    <UserId></UserId>
    <LogonType><LogonType>
    <DisplayName></DisplayName>
 </Principal>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





