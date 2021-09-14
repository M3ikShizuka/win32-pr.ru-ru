---
title: Иажентнотифисинк Рекуестстарт
description: Иажентнотифисинк Рекуестстарт
ms.assetid: acac2bf8-7472-4952-a984-a29654fb8b0b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 67ced12596114214cf712cef8dbbe81edb5af278
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342543"
---
# <a name="iagentnotifysinkrequeststart"></a>Иажентнотифисинк:: Рекуестстарт

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT RequestStart(
   long dwRequestID  // request ID
);                          
```

Уведомляет клиентское приложение о начале запроса.

-   Нет возвращаемого значения.

<dl> <dt>

<span id="dwRequestID"></span><span id="dwrequestid"></span><span id="DWREQUESTID"></span>*дврекуестид*
</dt> <dd>

Идентификатор запущенного запроса.

</dd> </dl>

Это событие позволяет контролировать, когда запрос в очереди начинается с идентификатора запроса.

## <a name="see-also"></a>См. также:

[**Иажентнотифисинк:: рекуесткомплете**](iagentnotifysink--requestcomplete.md), [**Иажент:: Load**](iagent--load.md), [**иажентчарактер:: Жестуреат**](iagentcharacter--gestureat.md), [**иажентчарактер:: Hide**](iagentcharacter--hide.md), [**IAgentCharacter:: Interrupt**](iagentcharacter--interrupt.md), [**IAgentCharacter:: MoveTo**](iagentcharacter--moveto.md), [**IAgentCharacter::P готовка**](iagentcharacter--prepare.md), [**IAgentCharacter::Pный макет**](iagentcharacter--play.md), [**IAgentCharacter:: Показать**](iagentcharacter--show.md), [**IAgentCharacter:: говорите**](iagentcharacter--speak.md), [**IAgentCharacter:: wait**](iagentcharacter--wait.md)


 

 




