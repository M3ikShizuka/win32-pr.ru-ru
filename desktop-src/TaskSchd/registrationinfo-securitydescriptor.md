---
title: Регистратионинфо. SecurityDescriptor, свойство
description: Для создания скриптов Возвращает или задает дескриптор безопасности задачи.
ms.assetid: e03607f0-c2a0-4aa1-a2b0-915b03aae968
keywords:
- планировщик задач свойства SecurityDescriptor
- Планировщик задач свойства SecurityDescriptor, объект Регистратионинфо
- Планировщик задач объекта Регистратионинфо, свойство SecurityDescriptor
topic_type:
- apiref
api_name:
- RegistrationInfo.SecurityDescriptor
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 379e42f41387a40b160a73ec3457d3d5b9feaf59
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172900"
---
# <a name="registrationinfosecuritydescriptor-property"></a>Регистратионинфо. SecurityDescriptor, свойство

Для создания скриптов Возвращает или задает дескриптор безопасности задачи. Если во время регистрации задачи был указан другой дескриптор безопасности, он заменит дескриптор безопасности, установленный этим свойством.

## <a name="syntax"></a>Синтаксис


```VB
RegistrationInfo.SecurityDescriptor As String
```



## <a name="property-value"></a>Значение свойства

Дескриптор безопасности, связанный с задачей.

## <a name="remarks"></a>Remarks

При чтении или записи XML-кода для задачи дескриптор безопасности задачи указывается с помощью элемента [**SecurityDescriptor**](taskschedulerschema-securitydescriptor-registrationinfotype-element.md) схемы планировщик задач.

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

 

 





