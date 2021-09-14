---
title: Регистратионинфо. Documentation, свойство
description: Для создания скриптов Возвращает или задает любую дополнительную документацию для задачи.
ms.assetid: 12ce9461-0cc7-49d0-8c57-7ff3ca32850a
keywords:
- планировщик задач свойств документации
- Свойство документации планировщик задач, объект Регистратионинфо
- Планировщик задач объекта Регистратионинфо, свойство Documentation
topic_type:
- apiref
api_name:
- RegistrationInfo.Documentation
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5832c78fae5c0ee9629077693db7e283369cc8af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172904"
---
# <a name="registrationinfodocumentation-property"></a>Регистратионинфо. Documentation, свойство

Для создания скриптов Возвращает или задает любую дополнительную документацию для задачи.

## <a name="syntax"></a>Синтаксис


```VB
RegistrationInfo.Documentation As String
```



## <a name="property-value"></a>Значение свойства

Любая дополнительная документация, связанная с задачей.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи дополнительная документация для задачи указывается с помощью элемента [**Documentation**](taskschedulerschema-documentation-registrationinfotype-element.md) схемы планировщик задач.

При задании значения этого свойства значением может быть текст, полученный из файла .dll ресурсов. Для ссылки на текст из файла ресурсов используется специализированная строка. Строка имеет формат $ (@ \[ DLL \] , \[ ResourceId \] ), где \[ Dll — это \] путь к .dll файлу, содержащему ресурс, а \[ ResourceId \] — идентификатор для текста ресурса. Например, при установке значения этого свойства в $ (@% SystemRoot% \\ System32 \\ResourceName.dll,-101) свойству будет присвоено значение текста ресурса с идентификатором, равным-101, в файле% SystemRoot% \\ system32 \\ResourceName.dll.

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

 

 





