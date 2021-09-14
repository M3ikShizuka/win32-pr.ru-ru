---
title: Доступ к удаленному реестру в 64-разрядном Windows
description: перенаправитель реестра обеспечивает удаленный доступ к реестру на 64-разрядной Windows с помощью функции регконнектрегистри.
ms.assetid: 7873c1e2-53fb-4c93-bf4c-251a13cd8db7
keywords:
- доступ к удаленному реестру 64-разрядное программирование Windows
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6a139198ca08e0fdb9d7bcb070dcabf89dfa5403
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127240913"
---
# <a name="remote-registry-access-in-64-bit-windows"></a>Доступ к удаленному реестру в 64-разрядном Windows

перенаправитель реестра обеспечивает удаленный доступ к реестру на 64-разрядной Windows с помощью функции [**регконнектрегистри**](/windows/desktop/api/winreg/nf-winreg-regconnectregistrya) .

Если клиент является 32-битным приложением, он обращается к представлению реестра по умолчанию в 32-битном сервере. Если клиент является 64-битным приложением, он обращается к представлению реестра с 64-битным реестром.

**Windows Server 2003:** Все клиенты получают доступ к 64-разрядному представлению реестра, если только приложение не использует \_ \_ флаг WOW64 32KEY. это поведение изменилось с Windows Server 2003 с пакетом обновления 1 (SP1) и Windows XP Professional x64 Edition при условии, что клиент и сервер работают под управлением этих версий Windows.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Перенаправитель реестра](registry-redirector.md)
</dt> <dt>

[Отражение реестра](registry-reflection.md)
</dt> </dl>

 

 