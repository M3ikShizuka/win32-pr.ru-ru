---
title: Присвоение имени файлу записи
description: Присвоение имени файлу записи
ms.assetid: fae2fd6a-4c2f-432f-a714-9faae6daeafe
keywords:
- макрос Капфилесеткаптурефиле
- макрос Капфилеаллок
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 47ea091a36777e176124689ba57be6c0fb75d07d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169655"
---
# <a name="naming-the-capture-file"></a>Присвоение имени файлу записи

В следующем примере используется макрос [**капфилесеткаптурефиле**](/windows/desktop/api/Vfw/nf-vfw-capfilesetcapturefile) , чтобы указать альтернативное имя файла (MYCAP.AVI) для файла записи и макроса [**капфилеаллок**](/windows/desktop/api/Vfw/nf-vfw-capfilealloc) , чтобы предварительно выделить файл размером 5 МБ.


```C++
char szCaptureFile[] = "MYCAP.AVI";

capFileSetCaptureFile( hWndC, szCaptureFile); 
capFileAlloc( hWndC, (1024L * 1024L * 5)); 
 
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




