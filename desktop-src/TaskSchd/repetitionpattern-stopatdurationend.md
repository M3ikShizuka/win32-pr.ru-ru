---
title: Репетитионпаттерн. Стопатдуратионенд, свойство
description: Для создания скриптов Возвращает или задает логическое значение, указывающее, останавливается ли работающий экземпляр задачи в конце шаблона повторения.
ms.assetid: 421f2d6f-7c35-44b4-97f2-45f46ca5e40e
keywords:
- планировщик задач свойства Стопатдуратионенд
- Планировщик задач свойства Стопатдуратионенд, объект Репетитионпаттерн
- Планировщик задач объекта Репетитионпаттерн, свойство Стопатдуратионенд
topic_type:
- apiref
api_name:
- RepetitionPattern.StopAtDurationEnd
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 20b95d7e8941a4249991692dffbd3cac9ad1ca7a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172859"
---
# <a name="repetitionpatternstopatdurationend-property"></a>Репетитионпаттерн. Стопатдуратионенд, свойство

Для создания скриптов Возвращает или задает логическое значение, указывающее, останавливается ли работающий экземпляр задачи в конце шаблона повторения.

## <a name="syntax"></a>Синтаксис


```VB
RepetitionPattern.StopAtDurationEnd As Boolean
```



## <a name="property-value"></a>Значение свойства

Логическое значение, указывающее, останавливается ли работающий экземпляр задачи в конце шаблона повторения.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи эти сведения указываются в элементе [**стопатдуратионенд**](taskschedulerschema-stopatdurationend-repetitiontype-element.md) схемы планировщик задач.

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

 

 





