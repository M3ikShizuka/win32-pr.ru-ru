---
description: После получения обработчика файла с помощью вызова функции Сетупопенфилекуеуе можно добавить файловые операции в очередь, файлы по файлу или постановку в очередь всех файлов в разделе INF.
ms.assetid: ba2f40cd-b0df-4768-8080-4fd80c50f2c2
title: Файлы очереди
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a73a05c9aef71e5707fd7814a4df1fdfa7cce4c1be5bed8a561dd0a0dc6de964
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119665434"
---
# <a name="queuing-files"></a>Файлы очереди

После получения обработчика файла с помощью вызова функции [**сетупопенфилекуеуе**](/windows/desktop/api/Setupapi/nf-setupapi-setupopenfilequeue) можно добавить файловые операции в очередь, файлы по файлу или постановку в очередь всех файлов в разделе INF.

Чтобы добавить операцию копирования для отдельного файла в очередь файлов, вызовите функцию [**сетупкуеуекопи**](/windows/desktop/api/Setupapi/nf-setupapi-setupqueuecopya) . Если требуется поставить в очередь операцию копирования файлов с использованием исходного носителя по умолчанию и целевых объектов, указанных в INF-файле, можно вызвать функцию [**сетупкуеуедефаулткопи**](/windows/desktop/api/Setupapi/nf-setupapi-setupqueuedefaultcopya) .

Можно добавить отдельный файл операция удаления или переименования в очередь открытия файлов, вызвав функцию [**сетупкуеуеделете**](/windows/desktop/api/Setupapi/nf-setupapi-setupqueuedeletea) или [**сетупкуеуеренаме**](/windows/desktop/api/Setupapi/nf-setupapi-setupqueuerenamea) .

 

 



