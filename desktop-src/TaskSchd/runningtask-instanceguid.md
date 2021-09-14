---
title: Руннингтаск. Инстанцегуид, свойство
description: Для создания скриптов возвращает идентификатор GUID для этого экземпляра задачи.
ms.assetid: 35be538f-5223-4c61-9491-677953b4135a
keywords:
- планировщик задач свойства Инстанцегуид
- Планировщик задач свойства Инстанцегуид, объект Руннингтаск
- Планировщик задач объекта Руннингтаск, свойство Инстанцегуид
topic_type:
- apiref
api_name:
- RunningTask.InstanceGuid
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 94f3ad40eb7c8799d12ca3b4a6aaeb0b968a9229
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172824"
---
# <a name="runningtaskinstanceguid-property"></a>Руннингтаск. Инстанцегуид, свойство

Для создания скриптов возвращает идентификатор GUID для этого экземпляра задачи.

## <a name="syntax"></a>Синтаксис


```VB
RunningTask.InstanceGuid As string
```



## <a name="property-value"></a>Значение свойства

Идентификатор GUID для этого экземпляра задачи. Идентификатор создается службой планировщик задач каждый раз при выполнении задачи.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





