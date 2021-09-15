---
title: Иаженткоммандсекс Жеселпконтекстид
description: Иаженткоммандсекс Жеселпконтекстид
ms.assetid: db5f93e9-8cd3-4147-94b4-50cfe12033c4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5a49a633a66622626973e450b9566033b1ad96e7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572887"
---
# <a name="iagentcommandsexgethelpcontextid"></a>Иаженткоммандсекс:: Жеселпконтекстид

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetHelpContextID(
   long * pulHelpID  // address of Commands object help topic ID
);
```

Получает [**хелпконтекстид**](helpcontextid-property.md) для объекта [**команды**](/windows/desktop/lwef/the-command-object) .

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="pulHelpID"></span><span id="pulhelpid"></span><span id="PULHELPID"></span>*пулхелпид*
</dt> <dd>

Адрес переменной, которая получает контекстный номер раздела справки для объекта [**команды**](/windows/desktop/lwef/the-command-object) .

</dd> </dl>

если вы создали файл справки Windows для приложения и настроили свойство [**HelpFile**](helpfile-property.md) символа, Microsoft Agent автоматически вызывает справку, когда [**хелпмодеон**](helpmodeon-property.md) имеет значение **True** и пользователь выбирает объект [**команды**](/windows/desktop/lwef/the-command-object) . Если в [**хелпконтекстид**](helpcontextid-property.md)имеется контекстный номер, агент вызывает справку и ищет раздел, определяемый текущим контекстным номером. Текущий контекстный номер — это значение **хелпконтекстид** для объекта **Command** .

Это свойство применяется только к символу, используемому вашим клиентским приложением. Этот параметр не влияет на другие клиенты символов или других символов клиентского приложения.

> [!Note]  
> для создания файла справки требуется компилятор справки Microsoft Windows.

 

## <a name="see-also"></a>См. также:

[**Иаженткоммандсекс:: сеселпконтекстид**](iagentcommandsex--sethelpcontextid.md), [**Иажентчарактерекс:: сеселпмодеон**](iagentcharacterex--sethelpmodeon.md), [**иажентчарактерекс:: SetHelpFileName**](iagentcharacterex--sethelpfilename.md)


 

 