---
title: Атрибут высоты VML V-and-Letter
description: Атрибут высоты VML V-and-Letter
ms.assetid: f06c0a50-1de1-47d8-8b94-01fe0599ed59
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 219d9f06e120ccc86bfa41c1cfff69b7feb64d68b1343732d45f57f26d952b21
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119864154"
---
# <a name="vml-v-same-letter-heights-attribute"></a>Атрибут высоты VML V-and-Letter

в этом разделе описывается функция VML, которая является устаревшей по отношению к Windows Internet Explorer 9. Веб-страницы и приложения, использующие VML, должны быть перенесены в формат SVG или другие широко поддерживаемые стандарты.

> [!Note]  
> По состоянию на Декабрь 2011 этот раздел был архивирован. В результате он больше не поддерживается. Дополнительные сведения см. в разделе [архивированное содержимое](/previous-versions/windows/internet-explorer/ie-developer/). сведения, рекомендации и рекомендации относительно текущей версии Windows Internet explorer см. в [центре разработчиков internet explorer](https://msdn.microsoft.com/ie/).

 

Определяет, будут ли все буквы иметь одинаковую высоту независимо от начального варианта. Read/write. **Вгтристате**.

**Применимо к**:

[текстпас](msdn-online-vml-textpath-element.md)

**Синтаксис тега**

<v: Style *элемента* = "v-та же буква-высота: *выражение* " >

**Синтаксис сценария**

*element* . Style. v-та же самая буква-высота = "*выражение*"

*выражение* = Высота *элемента*. Style. v-та же буква

**Замечания**

Если **значение равно true**, буквы в нижнем регистре растягиваются до высоты прописных букв. Значение по умолчанию равно **False**.

*Стандартный атрибут VML*

**Пример**

Все буквы будут одинаковой высотой, независимо от регистра.


```HTML
   <v:line from="50 100" to="400 100">
   <v:fill on="True" color="red"/>
   <v:path textpathok="True"/>
   <v:textpath on="True" string="VML Text"
   style="v-same-letter-heights:True;font:normal normal normal 36pt Arial"/>
   </v:line>
```



 

 