---
title: Регистратионинфо. URI, свойство
description: Для создания скриптов Возвращает или задает универсальный код ресурса (URI) задачи.
ms.assetid: 49085ee4-65e1-412c-ac1c-9c0f9efe5679
keywords:
- планировщик задач свойства URI
- Планировщик задач свойства URI, объект Регистратионинфо
- Планировщик задач объекта Регистратионинфо, свойство URI
topic_type:
- apiref
api_name:
- RegistrationInfo.URI
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 77598d556fdec29f41004529471c8098314a6faf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172896"
---
# <a name="registrationinfouri-property"></a>Регистратионинфо. URI, свойство

Для создания скриптов Возвращает или задает универсальный код ресурса (URI) задачи.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
RegistrationInfo.URI As String
```



## <a name="property-value"></a>Значение свойства

Универсальный код ресурса (URI) задачи.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи URI задачи указывается с помощью элемента [**URI**](taskschedulerschema-uri-registrationinfotype-element.md) схемы планировщик задач.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



 

 





