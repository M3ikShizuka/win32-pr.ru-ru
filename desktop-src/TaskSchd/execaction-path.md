---
title: Ексекактион. Path, свойство
description: Для создания скриптов Возвращает или задает путь к исполняемому файлу.
ms.assetid: 00fea05f-4f57-47ac-9812-8cd352fe02a8
keywords:
- Свойство пути планировщик задач
- Свойство Path планировщик задач, объект Ексекактион
- Планировщик задач объекта Ексекактион, свойство Path
topic_type:
- apiref
api_name:
- ExecAction.Path
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d363485db56634c39a4a12e153feb740b0c21a2b6a3ef9499754de753c6236f7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120011454"
---
# <a name="execactionpath-property"></a>Ексекактион. Path, свойство

Для создания скриптов Возвращает или задает путь к исполняемому файлу.

## <a name="syntax"></a>Синтаксис


```VB
ExecAction.Path As String
```



## <a name="property-value"></a>Значение свойства

Путь к исполняемому файлу, запускаемому действием.

## <a name="remarks"></a>Remarks

Это действие выполняет операцию командной строки. Например, действие может выполнить сценарий или запустить исполняемый файл.

При чтении или записи XML путь операции командной строки указывается в элементе [**Command**](taskschedulerschema-command-exectype-element.md) схемы планировщик задач.

Путь проверяется, чтобы убедиться, что он действителен при регистрации задачи, а не когда это свойство задано.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ексекактион**](execaction.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





