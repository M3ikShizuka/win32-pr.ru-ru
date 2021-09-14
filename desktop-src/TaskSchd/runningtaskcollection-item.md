---
title: Руннингтаскколлектион. Item, свойство
description: Для сценария возвращает указанную задачу из коллекции.
ms.assetid: 8b0745da-a11f-426c-9d52-f59d188e0e86
keywords:
- планировщик задач свойства элемента
- Свойство Item планировщик задач, объект Руннингтаскколлектион
- Планировщик задач объекта Руннингтаскколлектион, свойство Item
topic_type:
- apiref
api_name:
- RunningTaskCollection.Item
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 49d28da7a3f5348ff9f5d6171a1a698d95b646f0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886568"
---
# <a name="runningtaskcollectionitem-property"></a>Руннингтаскколлектион. Item, свойство

Для сценария возвращает указанную задачу из коллекции.

## <a name="syntax"></a>Синтаксис


```VB
RunningTaskCollection.Item( _
  ByVal Index _
) As RunningTask
```



## <a name="property-value"></a>Значение свойства

Объект [**руннингтаск**](runningtask.md) , содержащий запрошенный контекст.

## <a name="remarks"></a>Комментарии

Коллекции основаны на 1. Иными словами, индекс первого элемента в коллекции равен 1.

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

 

 





