---
title: Иажентчарактер
description: Иажентчарактер
ms.assetid: 6e8e3a68-a7bb-4afb-a753-836fe82a0b24
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6c812c7765bed791532db00c8f2e9cfd68cc771575e7a70fd27d45adef00bdb2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118478374"
---
# <a name="iagentcharactergetvisible"></a>Иажентчарактер:: Visible

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetVisible(
   long * pbVisible  // address of variable for character Visible setting
);
```

Определяет, видима ли в данный момент кадр анимации символа.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="pbVisible"></span><span id="pbvisible"></span><span id="PBVISIBLE"></span>*пбвисибле*
</dt> <dd>

Адрес переменной, принимающей **значение true** , если фрейм символа является видимым, и **false** , если он скрыт.

</dd> </dl>

С помощью этого метода можно определить, видима ли в данный момент рамка символа. Чтобы сделать символ видимым, используйте метод [**Показать**](/windows/desktop/lwef/iagentcharacter--show) . Чтобы скрыть символ, используйте метод [**Hide**](/windows/desktop/lwef/iagentcharacter--hide) .

 

 