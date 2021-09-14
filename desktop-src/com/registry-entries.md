---
title: Записи реестра (COM)
ms.assetid: f4f8875c-6416-4919-b49b-bcd675efcbd2
description: 'Дополнительные сведения о: записи реестра (COM)'
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 368e9eb5e4c2174c5b4b90df6586b58135085c5b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053137"
---
# <a name="registry-entries-com"></a>Записи реестра (COM)

Значения реестра в следующих разделах реестра управляют аспектами функциональности COM:

-   [**\_ \_ \\ Классы программного обеспечения для локального компьютера hKey \\**](hkey-local-machine-software-classes.md)
-   [**HKEY \_ по для локального \_ компьютера, \\ \\ Microsoft \\ OLE**](hkey-local-machine-software-microsoft-ole.md)
-   [**HKEY \_ \_ \\ программное обеспечение на локальном компьютере \\ Microsoft \\ Windows NT \\ CurrentVersion**](hkey-local-machine-software-microsoft-windows-nt-currentversion.md)

начиная с Windows Server 2003, COM использует только маркер текущего процесса, чтобы решить, к какому кусту реестра следует обращаться, а не к маркеру потока. Если COM не удается получить доступ к кусту реестра профиля пользователя, он будет обращаться к кусту **\_ локальной \_ машины \\** в разделе hKey.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Реестр](/windows/desktop/SysInfo/registry)
</dt> </dl>

 

 
