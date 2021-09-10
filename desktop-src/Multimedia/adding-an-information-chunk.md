---
title: Добавление информационного блока
description: Добавление информационного блока
ms.assetid: ebba5079-1f67-4236-9260-e36ff72ad51c
keywords:
- макрос Капфилесетинфочунк
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bacb99fb29e4b1882b4f257c428315f42ee3a360
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371340"
---
# <a name="adding-an-information-chunk"></a>Добавление информационного блока

Если необходимо включить в приложение другие сведения, помимо аудио и видео, можно создать фрагменты информации и вставить их в файл записи. Информационные блоки могут содержать несколько типов информации, включая сведения об авторских правах, идентификации источника видео или сведения о внешнем времени. В следующем примере хранятся сведения о внешнем времени — SMPTE (общество инженеров и телевизоров движения) в информационном фрагменте и добавляется в файл записи с помощью макроса [**капфилесетинфочунк**](/windows/desktop/api/Vfw/nf-vfw-capfilesetinfochunk) .


```C++
//  This example assumes the application controls 
//  the video source for preroll and postroll. 
CAPINFOCHUNK cic;
// . 
// . 
// . 
cic.fccInfoID = infotypeSMPTE_TIME;
cic.lpData = "00:20:30:12"; 
cic.cbData = strlen (cic.lpData) + 1;
capFileSetInfoChunk (hwndC, &cic); 
 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




