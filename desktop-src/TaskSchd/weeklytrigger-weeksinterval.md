---
title: Виклитригжер. Виксинтервал, свойство
description: Для создания скриптов Возвращает или задает интервал между неделями в расписании.
ms.assetid: 7992dee2-1725-4325-9fe9-eaff84fa5adc
keywords:
- планировщик задач свойства Виксинтервал
- Планировщик задач свойства Виксинтервал, объект Виклитригжер
- Планировщик задач объекта Виклитригжер, свойство Виксинтервал
topic_type:
- apiref
api_name:
- WeeklyTrigger.WeeksInterval
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4668b68d0b3f83e096284db35df799a63eb677b8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462596"
---
# <a name="weeklytriggerweeksinterval-property"></a>Виклитригжер. Виксинтервал, свойство

Для создания скриптов Возвращает или задает интервал между неделями в расписании.

## <a name="syntax"></a>Синтаксис


```VB
WeeklyTrigger.WeeksInterval As short
```



## <a name="property-value"></a>Значение свойства

Интервал между неделями в расписании.

## <a name="remarks"></a>Remarks

Чтобы запускать задание раз в неделю, укажите 1. Чтобы запускать задание раз в две недели, укажите 2.

При чтении или записи собственного XML-кода для задачи интервал для еженедельного расписания указывается с помощью элемента [**виксинтервал**](taskschedulerschema-weeksinterval-weeklyscheduletype-element.md) схемы планировщик задач.

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

 

 





