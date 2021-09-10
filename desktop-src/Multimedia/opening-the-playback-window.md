---
title: Открытие окна воспроизведения
description: Открытие окна воспроизведения
ms.assetid: 180f3fb9-cdcb-49ec-a708-84a597295b2f
keywords:
- Команда MCI_OPEN
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b6ea203c3a5d36ab747632b18b6550a3a0319159
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371736"
---
# <a name="opening-the-playback-window"></a>Открытие окна воспроизведения

В следующем примере показано, как использовать команду [**MCI \_ Open**](mci-open.md) , чтобы задать родительское окно и создать дочерний элемент этого окна.


```C++
MCI_DGV_OPEN_PARMS    mciOpen; 
 
mciOpen.lpstrElementName = lpstrFile;  // Set the filename.
mciOpen.dwStyle = WS_CHILD;            // Set the style. 
mciOpen.hWndParent = hWnd;             // Give a window handle. 
 
if (mciSendCommand(0, MCI_OPEN, 
   (DWORD)(MCI_OPEN_ELEMENT|MCI_DGV_OPEN_PARENT|MCI_DGV_OPEN), 
   (DWORD)(LPSTR)&mciOpen) == 0)
{ 
    // Open operation is successful. Continue. 
} 
```



 

 




