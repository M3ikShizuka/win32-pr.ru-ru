---
title: Атрибут точек VML
description: Атрибут точек VML
ms.assetid: 343d843e-9a09-4c89-af54-fb079129429b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8324bc22459b2991ff6360d661d85a2fcc52a4954d65307d2a5522033b7c0063
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119057742"
---
# <a name="vml-points-attribute"></a>Атрибут точек VML

в этом разделе описывается функция VML, которая является устаревшей по отношению к Windows Internet Explorer 9. Веб-страницы и приложения, использующие VML, должны быть перенесены в формат SVG или другие широко поддерживаемые стандарты.

> [!Note]  
> По состоянию на Декабрь 2011 этот раздел был архивирован. В результате он больше не поддерживается. Дополнительные сведения см. в разделе [архивированное содержимое](/previous-versions/windows/internet-explorer/ie-developer/). сведения, рекомендации и рекомендации относительно текущей версии Windows Internet explorer см. в [центре разработчиков internet explorer](https://msdn.microsoft.com/ie/).

 

Определяет набор точек, образующих ломаную линию. Read/write. [Ивгпоинтс](msdn-online-vml-ivgpoints-data-type.md) .

**Применимо к**:

[Ломаная линия](msdn-online-vml-polyline-element.md)

**Синтаксис тега**

<v: *element* Points = " *Expression* " >

**Синтаксис сценария**

*element* . Points = "*выражение * * *"**

*выражение* = *element*. Points

**Замечания**

Определяет набор прямых линейных сегментов, состоящих из нескольких точек. Если родительский элемент не является элементом VML, то [единицей](msdn-online-vml-units.md) по умолчанию является пиксель (но в нем также может быть указана система cm, mm, PT, PC). Значение по умолчанию — 0, 0 10, 10. Обратите внимание, что запятые не требуются, но они упрощают удобочитаемость.

*Стандартный атрибут VML*

**Пример**

Ломаная линия начинается в точке 10, 10 и заканчивается в 100 100, со значениями точек.


```HTML
   <v:polyline id="mypolyline"
   points="10pt,10pt 100pt,100pt">
   </v:polyline>
```



 

 