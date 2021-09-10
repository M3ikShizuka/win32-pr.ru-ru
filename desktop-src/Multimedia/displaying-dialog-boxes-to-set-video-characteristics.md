---
title: Отображение диалоговых окон для установки характеристик видео
description: Отображение диалоговых окон для установки характеристик видео
ms.assetid: 8074f7d1-e8ab-46c3-acc2-a18be0eb4cc7
keywords:
- Структура КАПДРИВЕРКАПС
- макрос Капдривержеткапс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 73eea12d69a3d23b0345bee3495d32cbb1ad0ffe
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371364"
---
# <a name="displaying-dialog-boxes-to-set-video-characteristics"></a>Отображение диалоговых окон для установки характеристик видео

Каждый драйвер записи может предоставить до трех различных диалоговых окон, используемых для управления аспектами обработки разрядов и отслеживания видео. В следующем примере показано, как отобразить эти диалоговые окна. Перед отображением каждого диалогового окна в примере вызывается макрос [**капдривержеткапс**](/windows/desktop/api/Vfw/nf-vfw-capdrivergetcaps) и проверяется Возвращаемая структура [**капдриверкапс**](/windows/win32/api/vfw/ns-vfw-capdrivercaps) , чтобы определить, может ли драйвер записи отобразить его.


```C++
HWND hWndC = capCreateCaptureWindow(TEXT("My Capture Window"),
    WS_CHILD | WS_VISIBLE, 0, 0, 160, 120, hwndParent, nID);

CAPDRIVERCAPS CapDriverCaps = { }; 
CAPSTATUS     CapStatus = { };

capDriverGetCaps(hWndC, &CapDriverCaps, sizeof(CAPDRIVERCAPS)); 
 
// Video source dialog box. 
if (CapDriverCaps.fHasDlgVideoSource)
{
    capDlgVideoSource(hWndC); 
}
 
// Video format dialog box. 
if (CapDriverCaps.fHasDlgVideoFormat) 
{
    capDlgVideoFormat(hWndC); 

    // Are there new image dimensions?
    capGetStatus(hWndC, &CapStatus, sizeof (CAPSTATUS));

    // If so, notify the parent of a size change.
} 
 
// Video display dialog box. 
if (CapDriverCaps.fHasDlgVideoDisplay)
{
    capDlgVideoDisplay(hWndC); 
}
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> <dt>

[**капдривержеткапс**](/windows/desktop/api/Vfw/nf-vfw-capdrivergetcaps)
</dt> </dl>

 

 




