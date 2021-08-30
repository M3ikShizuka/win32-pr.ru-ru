---
title: открытие Потоки в файле AVI и закрытие файла
description: открытие Потоки в файле AVI и закрытие файла
ms.assetid: 3c6afa04-3d95-48cd-b468-7167bac07d46
keywords:
- Функция Авифилежетстреам
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 634d1e21bc324c85636bd607e14669d3577b2b4b0b3296881af62baefb0b0db3
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120038304"
---
# <a name="opening-streams-in-an-avi-file-and-closing-the-file"></a>открытие Потоки в файле AVI и закрытие файла

Следующий пример открывает все потоки в файле AVI с помощью функции [**авифилежетстреам**](/windows/desktop/api/Vfw/nf-vfw-avifilegetstream) . Если возникает ошибка, файл закрывается.


```C++
// InsertAVIFile - opens the streams in an AVI file. 
// 
// pfile - file-interface pointer from AVIFileOpen 
// 
// Global variables 
// gcpavi - count of the number of streams in an AVI file 
// gapavi[] = array of stream-interface pointers 
 
void InsertAVIFile(PAVIFILE pfile, HWND hwnd, LPSTR lpszFile) 
{ 
    int    i; 
    gcpavi = 0; 
 
    // Open the streams until a stream is not available. 
    for (i = gcpavi; i < MAXNUMSTREAMS; i++) { 
        gapavi[i] = NULL; 
        if (AVIFileGetStream(pfile, &gapavi[i], 0L, i - gcpavi) 
            != AVIERR_OK) 
        break; 
 
    if (gapavi[i] == NULL) 
        break; 
    } 
    // Display error message-stream not found. 
    if (gcpavi == i) 
    { 
        // Handle failure.
        if (pfile) // If file is open, close it 
            AVIFileRelease(pfile); 
        return; 
    } 
    else { 
        gcpavi = i - 1; 
    } 
 
//  . 
//  . Place functions to process data here. 
//  . 
} 
 
```



 

 




