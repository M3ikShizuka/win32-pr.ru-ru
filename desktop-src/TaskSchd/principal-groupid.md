---
title: Свойство Principal. GroupId
description: Для создания скриптов Возвращает или задает идентификатор группы пользователей, необходимой для выполнения задач, связанных с участником.
ms.assetid: be0b7cd1-0e17-4aa5-af8e-880c95b3e7dc
keywords:
- Свойство GroupId планировщик задач
- Свойство GroupId планировщик задач, объект Principal
- Объект Principal планировщик задач, свойство GroupId
topic_type:
- apiref
api_name:
- Principal.GroupId
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bc7b5acd17d32b0123723fe53f91e390c37f42d2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173036"
---
# <a name="principalgroupid-property"></a>Свойство Principal. GroupId

Для создания скриптов Возвращает или задает идентификатор группы пользователей, необходимой для выполнения задач, связанных с участником.

## <a name="syntax"></a>Синтаксис


```VB
Principal.GroupId As String
```



## <a name="property-value"></a>Значение свойства

Идентификатор группы пользователей, связанной с этим участником.

## <a name="remarks"></a>Remarks

Не устанавливайте это свойство, если в свойстве [**UserID**](principal-userid.md) указан идентификатор пользователя.

При чтении или записи XML-кода для задачи идентификатор группы участника указывается в элементе [**groupId**](taskschedulerschema-groupid-principaltype-element.md) схемы планировщик задач.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**UserId**](principal-userid.md)
</dt> <dt>

[**Основного**](principal.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





