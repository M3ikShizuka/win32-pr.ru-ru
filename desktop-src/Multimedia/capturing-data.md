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
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272363"
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



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




