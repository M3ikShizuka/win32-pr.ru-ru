---
title: Свойство Triggered. Enabled
description: Для создания скриптов Возвращает или задает логическое значение, указывающее, включен ли триггер.
ms.assetid: 8fb5a0cc-ddd4-430d-9593-95a4cb311f18
keywords:
- Включенное свойство планировщик задач
- Включенное свойство планировщик задач, объект Trigger
- Триггер объекта планировщик задач, включенное свойство
topic_type:
- apiref
api_name:
- Trigger.Enabled
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 411bc36dcf03933e2b4cee2f575aaec3b8133846
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264915"
---
# <a name="triggerenabled-property"></a>Свойство Triggered. Enabled

Для создания скриптов Возвращает или задает логическое значение, указывающее, включен ли триггер.

## <a name="syntax"></a>Синтаксис


```VB
Trigger.Enabled As Boolean
```



## <a name="property-value"></a>Значение свойства

Значение true, если триггер включен; в противном случае — значение false. Значение по умолчанию — true.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи свойство Enabled задается с помощью элемента [**Enabled**](taskschedulerschema-enabled-triggerbasetype-element.md) схемы планировщик задач.

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

 

 





