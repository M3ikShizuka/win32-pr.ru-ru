---
title: Использование элементов PARAM на веб-странице, отображаемой Firefox
description: Использование элементов PARAM на веб-странице, отображаемой Firefox
ms.assetid: 8403c6f4-f221-4411-b49c-f0c9c22943df
keywords:
- проигрыватель Windows Media, элементы PARAM в элементе OBJECT
- проигрыватель Windows Media объектная модель, элементы PARAM в элементе object
- Объектная модель, элементы PARAM в элементе OBJECT
- проигрыватель Windows Media Мобильные, элементы PARAM в элементе OBJECT
- проигрыватель Windows Media ActiveX элемент управления, элементы PARAM в элементе OBJECT
- проигрыватель Windows Media мобильный ActiveX элемент управления, элементы PARAM в элементе OBJECT
- элемент управления ActiveX, элементы PARAM в элементе OBJECT
- внедрение, веб-страницы
- Внедрение веб-страниц, элементы PARAM в элементе OBJECT
- Элементы PARAM в элементе OBJECT
- проигрыватель Windows Media, Firefox
- объектная модель проигрыватель Windows Media, Firefox
- Объектная модель, Firefox
- проигрыватель Windows Media Mobile, Firefox
- проигрыватель Windows Media ActiveX элемент управления, Firefox
- проигрыватель Windows Media мобильный ActiveX элемент управления, Firefox
- ActiveX элемент управления, Firefox
- Firefox, элементы PARAM в элементе OBJECT
- Внедрение веб-страниц, Firefox
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6b045d111ff3cd0de09f54a8cf7ac25028fa1dc6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347703"
---
# <a name="using-param-elements-in-a-web-page-displayed-by-firefox"></a>Использование элементов PARAM на веб-странице, отображаемой Firefox

Элементы PARAM можно использовать внутри элемента OBJECT для задания начального состояния элемента управления проигрывателя. Например, элементы PARAM в следующем примере указывают, что элемент управления должен автоматически воспроизводиться в Сиэтле. WMV.


```HTML
<OBJECT id="Player" type="application/x-ms-wmp" width="300" height="200">
  <PARAM name="url" value="c:\MediaFiles\seattle.wmv" />
  <PARAM name="autostart" value="true" />
</OBJECT>

```



Большинство элементов PARAM можно интерпретировать с помощью Internet Explorer и Firefox. Однако существует несколько элементов PARAM, которые не поддерживаются подключаемым модулем Firefox. Сведения о том, какие элементы PARAM поддерживаются подключаемым модулем Firefox, см. [в разделе элементы param в ЭЛЕМЕНТЕ Object](param-elements-in-an-object-element.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**использование элемента управления проигрыватель Windows Media с браузером Firefox**](using-the-windows-media-player-control-with-firefox.md)
</dt> </dl>

 

 




