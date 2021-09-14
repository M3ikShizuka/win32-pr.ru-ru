---
title: Тасксеттингс. Рунонлифнетворкаваилабле, свойство
description: Для создания скриптов Возвращает или задает логическое значение, указывающее, что планировщик задач будет выполнять задачу только при доступности сети.
ms.assetid: 1a2b085f-0572-47d3-ac1f-0032c8427af0
keywords:
- планировщик задач свойства Рунонлифнетворкаваилабле
- Планировщик задач свойства Рунонлифнетворкаваилабле, объект Тасксеттингс
- Планировщик задач объекта Тасксеттингс, свойство Рунонлифнетворкаваилабле
topic_type:
- apiref
api_name:
- TaskSettings.RunOnlyIfNetworkAvailable
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8225d836e5bc87abd5ce9b6c311b4af527561d41
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145882"
---
# <a name="tasksettingsrunonlyifnetworkavailable-property"></a>Тасксеттингс. Рунонлифнетворкаваилабле, свойство

Для создания скриптов Возвращает или задает логическое значение, указывающее, что планировщик задач будет выполнять задачу только при доступности сети.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
TaskSettings.RunOnlyIfNetworkAvailable As Boolean
```



## <a name="property-value"></a>Значение свойства

Если значение — true, свойство указывает, что планировщик задач будет выполнять задачу только при доступности сети. Значение по умолчанию — False.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи этот параметр указывается в элементе [**рунонлифнетворкаваилабле**](taskschedulerschema-runonlyifnetworkavailable-settingstype-element.md) схемы планировщик задач.

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

 

 





