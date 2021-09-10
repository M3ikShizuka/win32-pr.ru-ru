---
title: Включение наложения видео
description: Включение наложения видео
ms.assetid: f0b4f24c-3e35-4a18-ac77-8cae7083b0fe
keywords:
- макрос Капдривержеткапс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7ce51a3b7c77fbb161007ddde7dfe91c36152121
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371370"
---
# <a name="enabling-video-overlay"></a>Включение наложения видео

В следующем примере с помощью макроса [**капдривержеткапс**](/windows/desktop/api/Vfw/nf-vfw-capdrivergetcaps) определяется, есть ли у драйвера записи возможности наложения. Если это так, макрос включает наложение.


```C++
CAPDRIVERCAPS CapDrvCaps; 

capDriverGetCaps(hWndC, &CapDrvCaps, sizeof (CAPDRIVERCAPS)); 

if (CapDrvCaps.fHasOverlay) 
    capOverlay(hWndC, TRUE);
 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




