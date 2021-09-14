---
title: Регистередтаск. Расчетное nextruntime, свойство
description: Для создания сценариев Возвращает время следующего запланированного выполнения зарегистрированной задачи.
ms.assetid: f63298a8-c9fa-4fea-ad0b-2c8739aced19
keywords:
- планировщик задач свойства расчетное nextruntime
- Планировщик задач свойства расчетное nextruntime, объект Регистередтаск
- Планировщик задач объекта Регистередтаск, свойство расчетное nextruntime
topic_type:
- apiref
api_name:
- RegisteredTask.NextRunTime
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 94db26c023ddd2c146586fbc433548517a84f234
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172983"
---
# <a name="registeredtasknextruntime-property"></a>Регистередтаск. Расчетное nextruntime, свойство

Для создания сценариев Возвращает время следующего запланированного выполнения зарегистрированной задачи.

## <a name="syntax"></a>Синтаксис


```VB
RegisteredTask.NextRunTime As String
```



## <a name="property-value"></a>Значение свойства

Время следующего запланированного выполнения зарегистрированной задачи.

## <a name="remarks"></a>Remarks

Если зарегистрированная задача содержит триггеры, которые по отдельности отключены, эти триггеры будут влиять на следующее запланированное время выполнения, которое возвращается, даже если они отключены.

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
</dt> <dt>

[**регистередтаск**](registeredtask.md)
</dt> </dl>

 

 





