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
ms.openlocfilehash: 2b9fe5439576322807abea6e10089460eaed4440496ed6a9e0f989dd44bc7e20
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120099704"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





