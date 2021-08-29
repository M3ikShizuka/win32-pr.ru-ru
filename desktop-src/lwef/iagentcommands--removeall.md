---
title: Иаженткоммандс RemoveAll
description: Иаженткоммандс RemoveAll
ms.assetid: fab43363-6325-4566-b7bb-599591f67321
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: dcb855a0eb4cd8a968ec5f03a37aa99fb170158cf75eec9f69a13c392ef94cdb
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118976284"
---
# <a name="iagentcommandsremoveall"></a>Иаженткоммандс:: RemoveAll

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT Remove();
```

Удаляет все [**команды**](/windows/desktop/lwef/the-command-object) из коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) .

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

Удаление всех [**команд**](/windows/desktop/lwef/the-command-object) из коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) также приводит к их удалению из всплывающего меню и **окна «Voice Commands»** , если приложение является входным. **RemoveAll** не удаляет записи сервера или другого клиента.

## <a name="see-also"></a>См. также:

[**Иаженткоммандс:: Add**](iagentcommands--add.md), [**Иаженткоммандс:: INSERT**](iagentcommands--insert.md), [**иаженткоммандс:: Remove**](iagentcommands--remove.md)


 

 