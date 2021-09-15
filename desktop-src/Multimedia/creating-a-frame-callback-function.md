---
title: Создание функции обратного вызова Frame
description: Создание функции обратного вызова Frame
ms.assetid: 37002ee0-9907-4aab-93cc-50fe9cd21cff
keywords:
- макрос Капсеткаллбакконфраме
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 07b2a921bfae235c50387c41865c44bb69b5c05a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461856"
---
# <a name="creating-a-frame-callback-function"></a>Создание функции обратного вызова Frame

В следующем примере показана простая функция обратного вызова Frame. Зарегистрируйте этот обратный вызов с помощью макроса [**капсеткаллбакконфраме**](/windows/desktop/api/Vfw/nf-vfw-capsetcallbackonframe) .


```
TCHAR gachBuffer[100];  // Global buffer.
DWORD gdwFrameNum = 0;

// FrameCallbackProc: frame callback function. 
// hWnd:              capture window handle. 
// lpVHdr:            pointer to structure containing captured 
//                        frame information. 
// 
LRESULT PASCAL FrameCallbackProc(HWND hWnd, LPVIDEOHDR lpVHdr) 
{ 
    if (!hWnd) 
        return FALSE; 
 
    _stprintf_s(gachBuffer, TEXT("Preview frame# %ld "), gdwFrameNum++); 
    SetWindowText(hWnd, gachBuffer); 
    return (LRESULT) TRUE ; 
} 
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




