---
title: Иаженткоммандсекс Жетглобалвоицекоммандсенаблед
description: Иаженткоммандсекс Жетглобалвоицекоммандсенаблед
ms.assetid: 9c8fa978-a02b-4dfc-8cf7-e066c5b75122
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 28aee044b9b25ff529a8c49943b6fd0bbb4d8175a5f3a9b6d482923170f4bdc5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119609494"
---
# <a name="iagentcommandsexgetglobalvoicecommandsenabled"></a>Иаженткоммандсекс:: Жетглобалвоицекоммандсенаблед

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetGlobalVoiceCommandsEnabled(
   long * pbEnabled  // address of the global voice command setting
);
```

Возвращает значение, указывающее, включена ли грамматика голоса для глобальных команд агента.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="pbEnabled"></span><span id="pbenabled"></span><span id="PBENABLED"></span>*пбенаблед*
</dt> <dd>

Адрес, который получает **значение true** , если включена грамматика голоса для глобальных команд агента, **значение false** , если отключено.

</dd> </dl>

Microsoft Agent автоматически добавляет параметры голоса (грамматики) для открытия и закрытия окна "Voice Commands", а также для отображения и скрытия символа. Когда этот метод возвращает **значение false**, все параметры голоса для этих команд, а также параметры голоса для [**заголовка**](caption-property.md) объектов [**команд**](/windows/desktop/lwef/the-command-object) других клиентов не включаются в грамматику. Это позволяет исключить их из текущей активной грамматики клиента. Однако этот параметр не отражает включение этих команд во всплывающем меню символа.

## <a name="see-also"></a>См. также:

[**Иаженткоммандсекс:: Сетглобалвоицекоммандсенаблед**](iagentcommandsex--setglobalvoicecommandsenabled.md)


 

 