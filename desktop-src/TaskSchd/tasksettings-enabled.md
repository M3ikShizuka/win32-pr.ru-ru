---
title: Тасксеттингс. Enabled, свойство
description: Для создания скриптов Возвращает или задает логическое значение, указывающее, что задача включена. Задачу можно выполнить, только если этот параметр имеет значение true.
ms.assetid: af8aa237-3402-4a82-b6ef-b713e1757d3a
keywords:
- Включенное свойство планировщик задач
- Включенное свойство планировщик задач, объект Тасксеттингс
- Планировщик задач объекта Тасксеттингс, свойство Enabled
topic_type:
- apiref
api_name:
- TaskSettings.Enabled
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6805d7b754ac2c3553d5fde91826ffa192b91d97
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968530"
---
# <a name="tasksettingsenabled-property"></a>Тасксеттингс. Enabled, свойство

Для создания скриптов Возвращает или задает логическое значение, указывающее, что задача включена. Задачу можно выполнить, только если этот параметр имеет значение true.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
TaskSettings.Enabled As Boolean
```



## <a name="property-value"></a>Значение свойства

Если задано значение true, задача включена. Если задано значение false, задача не включена.

## <a name="remarks"></a>Комментарии

При чтении или записи XML для задачи этот параметр указывается в элементе [**Enabled (сеттингстипе)**](taskschedulerschema-enabled-settingstype-element.md) схемы планировщик задач.

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

 

 





