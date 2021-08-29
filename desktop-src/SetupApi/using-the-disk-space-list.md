---
description: Прежде чем добавлять или удалять файловые операции из списка дискового пространства, необходимо создать его с помощью функции Сетупкреатедискспацелист.
ms.assetid: 287fd84a-dc8c-4a5c-b998-db5f2fbee5f1
title: Использование списка Disk-Space
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f715f9e62cc1cbd6019752ab1e7c7ebb365947736b15fd153767c01586ddb008
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119664594"
---
# <a name="using-the-disk-space-list"></a>Использование списка Disk-Space

Прежде чем добавлять или удалять файловые операции из списка дискового пространства, необходимо создать его с помощью функции [**сетупкреатедискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupcreatediskspacelista) .

После создания списка дискового пространства можно добавить отдельные операции копирования или удаления файлов в список с помощью [**сетупаддтодискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupaddtodiskspacelista). Чтобы добавить все операции копирования или удаления файлов во весь раздел INF, используйте функцию [**сетупаддсектионтодискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupaddsectiontodiskspacelista) или [**сетупаддинсталлсектионтодискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupaddinstallsectiontodiskspacelista) .

После добавления всех операций установки в список дискового пространства можно запросить его, чтобы узнать, сколько места на диске требуется для указанной установки с помощью функции [**сетупкуериспацерекуиредондриве**](/windows/desktop/api/Setupapi/nf-setupapi-setupqueryspacerequiredondrivea) .

Функция [**сетупкуеридривесиндискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupquerydrivesindiskspacelista) возвращает спецификации диска для каждого целевого диска, на который ссылается файловые операции в списке дискового пространства. Эти сведения можно использовать для программного сравнения доступного пространства на этих дисках с пространством, необходимым для установки.

Чтобы удалить файловую операцию из списка дискового пространства, используйте функцию [**сетупремовефромдискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupremovefromdiskspacelista) . Чтобы удалить все операции копирования или удаления файлов из всего раздела INF, используйте функцию [**сетупремовесектионфромдискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupremovesectionfromdiskspacelista) или [**сетупремовеинсталлсектионфромдискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupremoveinstallsectionfromdiskspacelista) .

После того как список дискового пространства больше не требуется, можно освободить ресурсы, выделенные для него, вызвав функцию [**сетупдестройдискспацелист**](/windows/desktop/api/Setupapi/nf-setupapi-setupdestroydiskspacelist) .

 

 



