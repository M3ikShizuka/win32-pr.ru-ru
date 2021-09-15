---
description: '\_Для выполнения сценария или приложения на удаленном компьютере можно использовать процесс Win32. Create. Однако в целях безопасности процесс не может быть интерактивным. Когда \_ на локальном компьютере вызывается Win32 Process. Create, процесс может быть интерактивным.'
ms.assetid: 11fea8b1-7d05-4f44-9103-ea804a1d4b38
ms.tgt_platform: multiple
title: Удаленное создание процессов с помощью WMI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 55e7b97f8f4fdddd608f6ee8c3368bde6ad6e854
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127575383"
---
# <a name="creating-processes-remotely-using-wmi"></a>Удаленное создание процессов с помощью WMI

Для выполнения сценария или приложения на удаленном компьютере можно использовать [**\_ процесс Win32. Create.**](/windows/desktop/CIMWin32Prov/create-method-in-class-win32-process) Однако в целях безопасности процесс не может быть интерактивным. Когда на локальном компьютере вызывается **Win32 \_ Process. Create** , процесс может быть интерактивным.

> [!WARNING]
> В этом разделе описывается общая процедура создания удаленного процесса с помощью инструментария WMI. если вы просто ищете запуск сценария в удаленной системе, см. раздел [подключение к инструментарию wmi удаленно с Windows Vista](connecting-to-wmi-remotely-starting-with-vista.md)или [подключение к wmi на удаленном компьютере с помощью Windows PowerShell](connecting-to-wmi-on-a-remote-computer-by-using-powershell.md). Дополнительные общие сведения об удаленном взаимодействии с помощью PowerShell см. в разделе [выполнение удаленных команд](https://technet.microsoft.com/library/dd819505.aspx).

 

Удаленный процесс не имеет пользовательского интерфейса, но он указан в **диспетчере задач**. Процесс, созданный локально, может выполняться под любой учетной записью, если у учетной записи есть разрешение на **выполнение метода Execute** для корневого \\ пространства имен CIMV2. Процесс, созданный удаленно, может выполняться под любой учетной записью, если у учетной записи есть **метод Execute** и разрешения **Remote Enable** для root \\ CIMV2. Разрешения **EXECUTE** и **Remote Enable** устанавливаются в элементе управления WMI на панели управления. Дополнительные сведения см. [в разделе Настройка безопасности пространства имен с помощью элемента управления WMI](setting-namespace-security-with-the-wmi-control.md).

Для удаленного создания интерактивного процесса можно использовать [**Win32 \_ ScheduledJob. Create**](/windows/desktop/CIMWin32Prov/create-method-in-class-win32-scheduledjob) . Но процессы, запущенные с помощью **Win32 \_ ScheduledJob. Create** , выполняются под учетной записью LocalSystem, которая может послужить слишком большим уровнем привилегий.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Защита удаленного WMI-подключения](securing-a-remote-wmi-connection.md)
</dt> <dt>

[Подключение к третьим компьютерам — делегирование](connecting-to-a-3rd-computer-delegation.md)
</dt> </dl>

 

 
