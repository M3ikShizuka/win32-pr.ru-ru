---
title: Получение состояния окна записи
description: Получение состояния окна записи
ms.assetid: 5095dbd2-7cd4-48b6-bbb4-1f0bddfcfd06
keywords:
- макрос Капжетстатус
- Структура КАПСТАТУС
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 01f848898247ad8ea2ddbb0dde7a13c08b6a7274
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371556"
---
# <a name="obtaining-the-status-of-a-capture-window"></a>Получение состояния окна записи

В следующем примере функция [SetWindowPos](/windows/win32/api/winuser/nf-winuser-setwindowpos) используется для установки размера окна отслеживания в соответствии с общими размерами входящего видеопотока на основе сведений, возвращаемых макросом [**Капжетстатус**](/windows/desktop/api/Vfw/nf-vfw-capgetstatus) в структуре [**капстатус**](/windows/win32/api/vfw/ns-vfw-capstatus) .


```C++
CAPSTATUS CapStatus;

capGetStatus(hWndC, &CapStatus, sizeof (CAPSTATUS)); 

SetWindowPos(hWndC, NULL, 0, 0, CapStatus.uiImageWidth, 
    CapStatus.uiImageHeight, SWP_NOZORDER | SWP_NOMOVE); 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 