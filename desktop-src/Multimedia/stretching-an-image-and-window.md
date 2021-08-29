---
title: Растяжение изображения и окна
description: Растяжение изображения и окна
ms.assetid: 661992eb-b012-47eb-84bc-cd12834c6270
keywords:
- Макрос МЦивнджетдест
- Макрос МЦивндпутдест
- Функция Жетвиндоврект
- Функция SetWindowPos
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a38cc3072be387f549e77186886854c8cf6a40a466ca5014c4eb85469faf762b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119781864"
---
# <a name="stretching-an-image-and-window"></a>Растяжение изображения и окна

Следующий пример растягивает изображения видеоклипа и изменяет пропорции отображаемых кадров. Фреймы, отображаемые в окне МЦивнд, являются вдвое высотой и в три раза больше ширины исходного кадра. Макросы [**мЦивнджетдест**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetdest) и [**мЦивндпутдест**](/windows/desktop/api/Vfw/nf-vfw-mciwndputdest) извлекают и переопределяют координаты прямоугольника назначения. Функции [жетвиндоврект](/windows/win32/api/winuser/nf-winuser-getwindowrect) и [SetWindowPos](/windows/win32/api/winuser/nf-winuser-setwindowpos) управляют изменениями в измерениях окна мЦивнд.


```C++
// extern RECT rCurrent, rDest; 
 
case WM_COMMAND: 
   switch (wParam) 
   { 
       case IDM_CREATEMCIWND: 
           g_hwndMCIWnd = MCIWndCreate(hwnd, 
           g_hinst, 
           WS_CHILD | WS_VISIBLE, 
          "sample.avi"); 
           break;    
 
       case IDM_RESIZEWINDOW: // destination RECT and playback area
           GetWindowRect(g_hwndMCIWnd, &rWin);     // window size 
           MCIWndGetDest(g_hwndMCIWnd, &rCurrent); // destination RECT
           rDest.top = rCurrent.top;               // new boundaries 
           rDest.right = rCurrent.right; 
           rDest.left = rCurrent.left + 
               ((rCurrent.left - rCurrent.right) * 3); 
           rDest.bottom = rCurrent.top + 
               ((rCurrent.bottom - rCurrent.top) * 2); 
           MCIWndPutDest(g_hwndMCIWnd, &rDest); // new RECT
           SetWindowPos(g_hwndMCIWnd,           // window to resize 
               NULL,                          // z-order: don't care 
               0, 0,                          // position: don't care
               rDest.right - rDest.left,      // width 
               (rWin.bottom - rWin.top +           // height (window - 
               (rCurrent.bottom - rCurrent.top) +  //  original RECT +
               (rDest.bottom - rDest.top)),        //  new RECT
               SWP_NOMOVE | SWP_NOZORDER | SWP_NOACTIVATE); 
           break; 
   } 
   break; 
 
   // Handle other messages here. 
```



 

 