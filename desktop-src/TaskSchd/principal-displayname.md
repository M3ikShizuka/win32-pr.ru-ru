---
title: Свойство Principal. DisplayName
description: Для создания скриптов Возвращает или задает имя участника.
ms.assetid: 73caf263-f597-4bea-ae89-32f9919d7a70
keywords:
- планировщик задач свойства DisplayName
- Свойство DisplayName планировщик задач, объект Principal
- Объект Principal планировщик задач, свойство DisplayName
topic_type:
- apiref
api_name:
- Principal.DisplayName
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 31a76ec9473bccb20ec484259ab8adfe26ad6441
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173043"
---
# <a name="principaldisplayname-property"></a>Свойство Principal. DisplayName

Для создания скриптов Возвращает или задает имя участника.

## <a name="syntax"></a>Синтаксис


```VB
Principal.DisplayName As String
```



## <a name="property-value"></a>Значение свойства

Имя участника.

## <a name="remarks"></a>Remarks

При чтении или записи XML для задачи отображаемое имя участника указывается в элементе [**DisplayName**](taskschedulerschema-displayname-principaltype-element.md) схемы планировщик задач.

При задании значения этого свойства значением может быть текст, полученный из файла .dll ресурсов. Для ссылки на текст из файла ресурсов используется специализированная строка. Строка имеет формат $ (@ \[ DLL \] , \[ ResourceId \] ), где \[ Dll — это \] путь к .dll файлу, содержащему ресурс, а \[ ResourceId \] — идентификатор для текста ресурса. Например, если задать для этого свойства значение $ (@% SystemRoot% \\ System32 \\ResourceName.dll,-101), в файле% SystemRoot% System32ResourceName.dll будет задано значение для свойства, равное-101 \\ \\ .

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
</dt> <dt>

[**Основного**](principal.md)
</dt> </dl>

 

 





