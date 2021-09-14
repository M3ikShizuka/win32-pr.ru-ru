---
title: Стопатдуратионенд (Репетитионтипе), элемент
description: Указывает, что выполняющиеся экземпляры задачи останавливаются в конце шаблона повторения.
ms.assetid: 4e34b5b2-ac93-4951-9de4-3e89614517d1
keywords:
- планировщик задач элемента Стопатдуратионенд
topic_type:
- apiref
api_name:
- StopAtDurationEnd
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a95f15f3a62d05b9bc28dc9f50b924979e2b748c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968646"
---
# <a name="stopatdurationend-repetitiontype-element"></a>Стопатдуратионенд (Репетитионтипе), элемент

Указывает, что выполняющийся экземпляр задачи останавливается в конце срока действия шаблона повторения. Это применимо только в том случае, если заданы повторения.

``` syntax
<xs:element name="StopAtDurationEnd"
 type="boolean"
 />
```

Элемент **стопатдуратионенд** определяется сложным типом [**репетитионтипе**](taskschedulerschema-repetitiontype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент

| Элемент | Унаследован от | Описание |
|-|-|-|
| [**Повторение**](taskschedulerschema-repetition-triggerbasetype-element.md) | [**репетитионтипе**](taskschedulerschema-repetitiontype-complextype.md) | Указывает, как часто выполняется задача и как долго шаблон повторения повторяется после запуска задачи.<br/> |

## <a name="remarks"></a>Комментарии

Для разработки сценариев этот параметр указывается с помощью свойства [**репетитионпаттерн. стопатдуратионенд**](repetitionpattern-stopatdurationend.md) .

Для разработки на C++ этот параметр указывается с помощью свойства [**ирепетитионпаттерн:: стопатдуратионенд**](/windows/win32/api/taskschd/nf-taskschd-irepetitionpattern-get_stopatdurationend) .

## <a name="requirements"></a>Требования

| Требование | Значение |
|-|-|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/> |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |

## <a name="see-also"></a>См. также раздел

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)

[Планировщик заданий](task-scheduler-start-page.md)
