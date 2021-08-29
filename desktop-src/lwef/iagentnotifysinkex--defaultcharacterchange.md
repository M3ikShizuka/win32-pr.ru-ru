---
title: Иажентнотифисинкекс Дефаултчарактерчанже
description: Иажентнотифисинкекс Дефаултчарактерчанже
ms.assetid: 13acb502-e247-433f-abf3-2d78a2d6a4a7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b2aea2a310e55228f6e9f15ec14f9ed9ac6e20374f8c8ecb12e016d60f1809b0
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119961474"
---
# <a name="iagentnotifysinkexdefaultcharacterchange"></a>Иажентнотифисинкекс::D Ефаултчарактерчанже

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT DefaultCharacterChange(
   BSTR bszGUID  // character identifier
);
```

Уведомляет клиентское приложение об изменении символа по умолчанию.

-   Нет возвращаемого значения.

<dl> <dt>

<span id="bszGUID"></span><span id="bszguid"></span><span id="BSZGUID"></span>*бсзгуид*
</dt> <dd>

Уникальный идентификатор для символа.

</dd> </dl>

Когда пользователь изменяет символ, назначенный в качестве символа по умолчанию для пользователя, сервер отправляет это событие клиентам, которые загрузили символ по умолчанию. Событие возвращает уникальный идентификатор (GUID) символа, отформатированный с помощью фигурных скобок и дефисов, который определяется при построении символа с помощью редактора символов Microsoft Agent.

Когда появляется новый символ, он предполагает тот же размер, что и любой уже загруженный экземпляр символа или предыдущий символ по умолчанию (в указанном порядке).

## <a name="see-also"></a>См. также:

[**Иажент:: Load**](iagent--load.md)


 

 




