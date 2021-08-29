---
title: Иаженткоммандс добавить
description: Иаженткоммандс добавить
ms.assetid: f6be7773-77fa-4c59-8feb-c2ebf54fd2e0
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4cd466290f8e12adc00986aa83a63ca9ba4ce46b4c7e13b8c368cdff1d14a4a2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118750214"
---
# <a name="iagentcommandsadd"></a>Иаженткоммандс:: Add

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT Add(
   BSTR bszCaption,  // Caption setting for Command
   BSTR bszVoice,    // Voice setting for Command
   long bEnabled,    // Enabled setting for Command
   long bVisible,    // Visible setting for Command
   long * pdwID      // address for variable for ID
);
```

Добавляет [**команду**](/windows/desktop/lwef/the-command-object) в коллекцию [**Commands**](/windows/desktop/lwef/the-commands-collection-object) .

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="bszCaption"></span><span id="bszcaption"></span><span id="BSZCAPTION"></span>*бсзкаптион*
</dt> <dd>

Объект BSTR, указывающий значение текста [**заголовка**](caption-property.md) , отображаемого для [**команды**](/windows/desktop/lwef/the-command-object) в коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) .

</dd> <dt>

<span id="bszVoice"></span><span id="bszvoice"></span><span id="BSZVOICE"></span>*бсзвоице*
</dt> <dd>

Объект BSTR, указывающий значение параметра текста [**голоса**](voice-property.md) для [**команды**](/windows/desktop/lwef/the-command-object) в коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) .

</dd> <dt>

<span id="bEnabled"></span><span id="benabled"></span><span id="BENABLED"></span>*бенаблед*
</dt> <dd>

Логическое выражение, задающее параметр [**Enabled**](enabled-property.md) для [**команды**](/windows/desktop/lwef/the-command-object) в коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) . Если параметр имеет **значение true**, **команда** включена и может быть выбрана. Если задано **значение false**, **команда** отключена.

</dd> <dt>

<span id="bVisible"></span><span id="bvisible"></span><span id="BVISIBLE"></span>*бвисибле*
</dt> <dd>

Логическое выражение, указывающее [**видимый**](visible-property.md) параметр для [**команды**](/windows/desktop/lwef/the-command-object) в коллекции [**команд**](/windows/desktop/lwef/the-commands-collection-object) . Если параметр имеет **значение true**, **команда** будет видна во всплывающем меню символа (если также задано свойство [**Caption**](caption-property.md) ).

</dd> <dt>

<span id="pdwID_"></span><span id="pdwid_"></span><span id="PDWID_"></span>*пдвид* 
</dt> <dd>

Адрес переменной, которая получает идентификатор для добавленной [**команды**](/windows/desktop/lwef/the-command-object).

</dd> </dl>

## <a name="see-also"></a>См. также

[**Иаженткомманд:: сеткаптион**](iagentcommand--setcaption.md), [**Иаженткомманд:: сетенаблед**](iagentcommand--setenabled.md), [**иаженткомманд:: Сетвисибле**](iagentcommand--setvisible.md), [**иаженткомманд:: SetVoice**](iagentcommand--setvoice.md), [**IAgentCommands:: INSERT**](iagentcommands--insert.md), [**IAgentCommands:: Remove**](iagentcommands--remove.md), [**IAgentCommands:: RemoveAll**](iagentcommands--removeall.md)


 

 