---
title: Атрибут StartAngle в формате VML
description: Атрибут StartAngle в формате VML
ms.assetid: 334ae52a-cde4-427e-8080-ec789b4d9d39
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b7237c20acb3e2b9a5b2445dc1ffed4e23a93bb55958831f5607410cde092dbe
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119796164"
---
# <a name="vml-startangle-attribute"></a>Атрибут StartAngle в формате VML

в этом разделе описывается функция VML, которая является устаревшей по отношению к Windows Internet Explorer 9. Веб-страницы и приложения, использующие VML, должны быть перенесены в формат SVG или другие широко поддерживаемые стандарты.

> [!Note]  
> По состоянию на Декабрь 2011 этот раздел был архивирован. В результате он больше не поддерживается. Дополнительные сведения см. в разделе [архивированное содержимое](/previous-versions/windows/internet-explorer/ie-developer/). сведения, рекомендации и рекомендации относительно текущей версии Windows Internet explorer см. в [центре разработчиков internet explorer](https://msdn.microsoft.com/ie/).

 

Определяет начальную точку дуги. Чтение и запись. [Вганглеиндегрис](msdn-online-vml-vgangleindegrees-data-type.md) .

**Применимо к**:

[Arc](msdn-online-vml-arc-element.md)

**Синтаксис тега**

<v: *element* ендангле = " *выражение* " >

**Синтаксис сценария**

*element* . ендангле = "*выражение*"

*выражение* = *element*. ендангле

**Замечания**

Дуга определяется как штрих, нарисованный вдоль овала, ограниченного атрибутами **стиля** фигуры. Начало штриха определяется углом, измеренным с начала (12 часов) по часовой стрелке. Значение по умолчанию — 0 градусов.

Стандартный атрибут VML

**Пример**

Дуга является улыбкой. Начальная точка находится на точке 90 градусов вписанный внутри прямоугольника, ограничивающего фигуру. Конечная точка находится в точке овала в 270 градусов.


```HTML
   <v:arc id="myarc"
   style="position:relative;top:10;left:10;width:200;height:200"
   startangle="90" endangle="270">
   </v:arc>
```



 

 