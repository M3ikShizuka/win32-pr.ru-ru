---
title: Пример раздела точечного рисунка
description: Пример раздела точечного рисунка
ms.assetid: 51b84b34-3cbb-4863-b7dc-e33e80d6ba23
keywords:
- проигрыватель Windows Media Обложки для мобильных устройств, точечные рисунки
- обложки, точечные рисунки
- Справочник по обложкам, точечным рисункам
- точечные рисунки в обложках, раздел точечных рисунков
- файлы определения обложки, раздел растровых изображений
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 00b05183be7ba56ed5b00a6bfd26ee6162e008cd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064339"
---
# <a name="sample-bitmap-section"></a>Пример раздела точечного рисунка

В следующих строках показан типичный раздел точечных рисунков в файле определения обложки:


```C++
[ Bitmaps ]

//  <Type>      <File name>     <X,Y>
//  ------      -----------     -----
    Background  Background.bmp  0,0
    Disabled    Disabled.bmp    0,0
    Pushed      Pushed.bmp      0,0
    Region      Region.bmp      0,0
    Super       Super.bmp       0,0
    

```



Он определяет пять растровых изображений, которые используются для создания фонового изображения, изображения для отключенных и отправленных кнопок, изображение региона для кнопок области и супер-изображение для значений TrackBar.

> [!Note]  
> в обложках для проигрыватель Windows Media 10 Mobile или более поздней версии не рекомендуется использовать область и супер bitmap.

 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Растровые изображения**](bitmaps.md)
</dt> </dl>

 

 




