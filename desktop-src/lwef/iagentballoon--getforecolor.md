---
title: Иажентбаллун
description: Иажентбаллун
ms.assetid: b06ad924-66b6-42a6-8c97-5bc4c46f6e2d
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: fabd35a43cba0485bbda1fae20b116316dec90832e42920d010b27586e972c5f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119962334"
---
# <a name="iagentballoongetforecolor"></a>Иажентбаллун::/ForeColor

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetForeColor(
   long * plFGColor // address of variable for foreground color displayed
);                  // in word balloon
```

Извлекает значение цвета переднего плана, отображаемого в окне всплывающей подсказки.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="plFGColor"></span><span id="plfgcolor"></span><span id="PLFGCOLOR"></span>*плфгколор*
</dt> <dd>

Адрес переменной, получающей параметр цвета для переднего плана.

</dd> </dl>

Цвет переднего плана, используемый в подсказке для символьного слова, определен в редакторе символов Microsoft Agent. Оно не может быть изменено приложением. Однако пользователь может переопределить цвет переднего плана для всех символов на странице свойств Microsoft Agent.

## <a name="see-also"></a>См. также:

[**Иажентбаллун:: Жетбаккколор**](iagentballoon--getbackcolor.md)


 

 




