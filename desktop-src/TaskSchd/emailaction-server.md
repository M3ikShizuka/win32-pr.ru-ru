---
title: Емаилактион. Server, свойство
description: Для создания скриптов Возвращает или задает имя SMTP-сервера, который используется для отправки электронной почты.
ms.assetid: a6e03144-ae3e-4c4c-aad8-884be5ab324f
keywords:
- планировщик задач свойств сервера
- Свойство сервера планировщик задач, объект Емаилактион
- Планировщик задач объекта Емаилактион, свойство сервера
topic_type:
- apiref
api_name:
- EmailAction.Server
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0fefcc5e33727d6b4ad0bcd60e48432c68422105
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462624"
---
# <a name="emailactionserver-property"></a>Емаилактион. Server, свойство

\[Этот объект больше не поддерживается. Используйте Иексекактион с командлетом PowerShell [**Send-MailMessage**](/powershell/module/microsoft.powershell.utility/send-mailmessage) в качестве обходного пути.\]

Для создания скриптов Возвращает или задает имя SMTP-сервера, который используется для отправки электронной почты.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
EmailAction.Server As String
```



## <a name="property-value"></a>Значение свойства

Имя сервера, который используется для отправки электронной почты.

## <a name="remarks"></a>Remarks

Убедитесь, что SMTP-сервер, который отправляет сообщение, правильно настроен. электронная почта отправляется с использованием проверки подлинности NTLM для Windows SMTP-серверов. это означает, что учетные данные безопасности, используемые для выполнения задачи, также должны иметь права доступа на SMTP-сервере для отправки сообщения электронной почты. если SMTP-сервер является сервером, отличным от Windows, то сообщение электронной почты будет отправлено, если сервер разрешает анонимный доступ. Сведения о настройке SMTP-сервера см. в разделе [Настройка SMTP-](https://www.microsoft.com/technet/prodtechnol/WindowsServer2003/Library/IIS/e4cf06f5-9a36-474b-ba78-3f287a2b88f2.mspx?mfr=true)сервера, а сведения об управлении параметрами SMTP-сервера см. в разделе [Администрирование SMTP](/previous-versions/windows/it-pro/windows-server-2003/cc758258(v=ws.10)).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                    |
| Поддержка конца сервера<br/>    | Windows Server 2008 R2<br/>                                                       |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**емаилактион**](emailaction.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

