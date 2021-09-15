---
description: 'выпуск VSS Windows Server 2003 больше не поддерживает следующее:'
ms.assetid: 01993cae-433e-4d01-b805-f97592369575
title: функции, удаленные с Windows Server 2003
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 181d053420f0fc947ebad024c0eaf2bbaf32f3e6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461327"
---
# <a name="functionality-removed-from-windows-server-2003"></a>функции, удаленные с Windows Server 2003

выпуск VSS Windows Server 2003 больше не поддерживает следующее:

-   Модули записи не могут указывать новые назначения восстановления файлов ([*новые целевые расположения*](vssgloss-n.md)) в операциях восстановления.
-   Повторное подключение доступной теневой копии в качестве тома с возможностью записи больше не поддерживается. Метод **ивссбаккупкомпонентс:: ремаунтреадврите** больше не доступен.
-   Модули записи не могут указывать явно включаемые файлы (с помощью [**ивсскреатевритерметадата:: аддинклудефилес**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-addincludefiles)). Файлы можно добавлять в компонент только в составе набора файлов с помощью [**ивсскреатевритерметадата:: аддфилестофилеграуп**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-addfilestofilegroup), [**Ивсскреатевритерметадата:: адддатабасефилес**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-adddatabasefiles)или [**IVssCreateWriterMetadata:: AddDatabaseLogFiles**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-adddatabaselogfiles).

    Файлы по-прежнему можно явно исключить из компонента с помощью [**ивсскреатевритерметадата:: аддексклудефилес**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-addexcludefiles).

 

 



