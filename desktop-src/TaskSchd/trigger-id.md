---
title: Trigger.Id, свойство
description: Для создания скриптов Возвращает или задает идентификатор триггера.
ms.assetid: 15dd3aaa-f3ee-459d-a0bd-327c7a4beb03
keywords:
- Свойство ID планировщик задач
- Свойство ID планировщик задач, объект Trigger
- Планировщик задач объекта триггера, свойство ID
topic_type:
- apiref
api_name:
- Trigger.Id
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 91a3868f76368b19e6a316b222b8ddaf4cbbff96
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264904"
---
# <a name="triggerid-property"></a>Trigger.Id, свойство

Для создания скриптов Возвращает или задает идентификатор триггера.

## <a name="syntax"></a>Синтаксис


```VB
Trigger.Id As String
```



## <a name="property-value"></a>Значение свойства

Идентификатор триггера. Этот идентификатор используется планировщик задач в целях ведения журнала.

## <a name="remarks"></a>Remarks

При чтении или записи XML-кода для задачи Идентификатор триггера задается в атрибуте ID отдельных элементов Trigger (например, атрибут ID элемента [**буттригжер**](taskschedulerschema-boottrigger-triggergroup-element.md) ) схемы планировщик задач.

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

 

 





