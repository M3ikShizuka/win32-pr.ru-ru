---
title: Иажентбаллун Жетнумчарсперлине
description: Иажентбаллун Жетнумчарсперлине
ms.assetid: ae0c7fff-8c58-465e-9b4f-3260f7574b57
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 62415c5e51cbf6642b4a348de2060fccb6bac41467dd00b7671888d06b8e71f8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119888403"
---
# <a name="iagentballoongetnumcharsperline"></a>Иажентбаллун:: Жетнумчарсперлине

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetNumCharsPerLine(
   long * plCharsPerLine  // address of variable for characters per line
);                        // displayed in word balloon
```

Возвращает значение для среднего количества символов в строке, отображаемых в подсказке к слову.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="pbCharsPerLine"></span><span id="pbcharsperline"></span><span id="PBCHARSPERLINE"></span>*пбчарсперлине*
</dt> <dd>

Адрес переменной, которая получает количество символов в строке.

</dd> </dl>

Сервер Microsoft Agent автоматически прокручивает строки, отображаемые для речевого вывода, в окне всплывающей программы. Среднее число символов в строке для всплывающего слова символа определяется в редакторе символов Microsoft Agent. Оно не может быть изменено приложением.

## <a name="see-also"></a>См. также:

[**Иажентбаллун:: Жетнумлинес**](iagentballoon--getnumlines.md)


 

 




