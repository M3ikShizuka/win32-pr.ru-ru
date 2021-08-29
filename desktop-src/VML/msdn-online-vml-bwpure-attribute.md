---
title: Атрибут Бвпуре VML
description: Атрибут Бвпуре VML
ms.assetid: a68e8197-bfd6-4b8e-8d4c-598590addff8
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 80b06c53ddc6279d16eeeaaed40a87794a1ab06d8b282ce4eef12a0e1bd74e35
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118999304"
---
# <a name="vml-bwpure-attribute"></a>Атрибут Бвпуре VML

в этом разделе описывается функция VML, которая является устаревшей по отношению к Windows Internet Explorer 9. Веб-страницы и приложения, использующие VML, должны быть перенесены в формат SVG или другие широко поддерживаемые стандарты.

> [!Note]  
> По состоянию на Декабрь 2011 этот раздел был архивирован. В результате он больше не поддерживается. Дополнительные сведения см. в разделе [архивированное содержимое](/previous-versions/windows/internet-explorer/ie-developer/). сведения, рекомендации и рекомендации относительно текущей версии Windows Internet explorer см. в [центре разработчиков internet explorer](https://msdn.microsoft.com/ie/).

 

Определяет режим черно-белого цвета для чистых и белых выходных устройств. Read/write. [Вгблакквхитемоде](msdn-online-vml-vgblackwhitemode.md).

**Применимо к**:

[Фигура](shape-element--vml.md)

**Синтаксис тега**

<v: *element* о:бвпуре = " *выражение* " >

**Замечания**

Если для [бвмоде](msdn-online-vml-bwmode-attribute.md) задано значение **Auto**, этот атрибут используется для определения способа отрисовки фигуры в чисто черном и белом режиме.

Дополнительные сведения о значениях этого атрибута см. в разделе [вгблакквхитемоде](msdn-online-vml-vgblackwhitemode.md) . Значение по умолчанию — **Auto**.

*Microsoft Office Extensions, атрибут*

**Пример**

Фигура обрабатывается как изображение с высокой контрастностью для выходных данных чистого черного и белого.


```HTML
   <v:rect id=myrect fillcolor="red" o:bwpure="highcontrast" o:bwmode="auto"
   style="position:relative;top:1;left:1;width:20;height:20">
   </v:rect>
```



 

 