---
title: Атрибут Алсреф (Имажедата) (VML)
description: Атрибут Алсреф (Имажедата) (VML)
ms.assetid: c55ede90-3d57-4f27-9940-1fe4751cef71
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ca832ab684c2f3dd2efaa6b34343df11be75118cc797b16fece671d430f866fa
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119137067"
---
# <a name="althref-attribute-imagedatavml"></a>Атрибут Алсреф (Имажедата) (VML)

в этом разделе описывается функция VML, которая является устаревшей по отношению к Windows Internet Explorer 9. Веб-страницы и приложения, использующие VML, должны быть перенесены в формат SVG или другие широко поддерживаемые стандарты.

> [!Note]  
> По состоянию на Декабрь 2011 этот раздел был архивирован. В результате он больше не поддерживается. Дополнительные сведения см. в разделе [архивированное содержимое](/previous-versions/windows/internet-explorer/ie-developer/). сведения, рекомендации и рекомендации относительно текущей версии Windows Internet explorer см. в [центре разработчиков internet explorer](https://msdn.microsoft.com/ie/).

 

Указывает альтернативную ссылку для изображения. Read/write. **Строка**.

**Применимо к**:

[ImageData](msdn-online-vml-imagedata-element.md)

**Синтаксис тега**

<v: *element* о:алсреф = " *выражение* " >

**Синтаксис сценария**

*element* . алсреф = "*выражение*"

*выражение* = *element*. алсреф

**Замечания**

Поддерживает сохранение данных PICT через HTML переносе. При записи в формате HTML альтернативное представление (то есть исходные данные PICT, если файл был создан из Macintosh) сохраняется. При чтении HTML **алсреф** имеет приоритет над **src**.

*Microsoft Office Extensions, атрибут*

 

 