---
title: легацисекуререференцес
description: Определяет, защищены ли вызовы AddRef/Release для приложений, которые не вызывают CoInitializeSecurity.
ms.assetid: 955b599b-1858-475a-95c4-a55038a28e69
keywords:
- COM-значение реестра Легацисекуререференцес
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2776bf3661013f1e622bbc2e1c553f2551c62808
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369653"
---
# <a name="legacysecurereferences"></a>легацисекуререференцес

Определяет  / , защищены ли вызовы **выпуска** AddRef для приложений, которые не вызывают [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity).

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Ole
   LegacySecureReferences = value
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ SZ** . Значение "Y" или "y" указывает, что **AddRef** и **Release** защищены. Если это значение реестра отсутствует или имеет значение, отличное от "Y" или "y", **AddRef** и **Release** не защищаются. Включение защиты ссылок снижает производительность удаленных вызовов.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Регистрация серверов COM](registering-com-servers.md)
</dt> <dt>

[Настройка безопасности на уровне процесса](setting-processwide-security.md)
</dt> </dl>

 

 




