---
title: Запись данных
description: Запись данных
ms.assetid: de029673-9929-40f9-b29b-2598e1e5c988
keywords:
- макрос Капкаптуресекуенце
- макрос Капфилесавеас
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f24b2110da9a85faaa991e67efdd1ef48e3d9c29
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371346"
---
# <a name="capturing-data"></a>Запись данных

В следующем примере используется макрос [**капкаптуресекуенце**](/windows/desktop/api/Vfw/nf-vfw-capcapturesequence) для запуска видеозаписи и макроса [**капфилесавеас**](/windows/desktop/api/Vfw/nf-vfw-capfilesaveas) для копирования записанных данных из файла записи в файл NEWFILE.AVI.


```C++
char szNewName[] = "NEWFILE.AVI";

// Set up the capture operation.

capCaptureSequence(hWndC); 

// Capture.

capFileSaveAs(hWndC, szNewName); 
 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




