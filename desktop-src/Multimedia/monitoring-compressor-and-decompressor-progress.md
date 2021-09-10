---
title: Мониторинг хода выполнения программы сжатия и распаковки
description: Мониторинг хода выполнения программы сжатия и распаковки
ms.assetid: 7c87c688-75b6-4d3e-9dd5-5f509ff2e473
keywords:
- Диспетчер сжатия видео (ВКМ), мониторинг
- ВКМ (диспетчер сжатия видео), мониторинг
- Функция Иксетстатуспрок
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: beb86a40bb653380dc93e758ada1b2eef6ec9ca7
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370398"
---
# <a name="monitoring-compressor-and-decompressor-progress"></a>Мониторинг хода выполнения программы сжатия и распаковки

В следующем примере показано, как использовать функцию [**иксетстатуспрок**](/windows/desktop/api/Vfw/nf-vfw-icsetstatusproc) для информирования программы сжатия или декомпрессора адреса функции обратного вызова.


```C++
ICSetStatusProc(compvars.hic, 0, (LPARAM) (UINT) hwndApp, 
    &PreviewStatusProc); 
 
```



В следующем примере показана функция обратного вызова, установленная предыдущим фрагментом:


```C++
LONG CALLBACK export PreviewStatusProc(LPARAM lParam, 
    UINT message, LONG l) 
{ 
    switch (message) 
    { 
        MSG msg; 
        case ICSTATUS_START: 
         
        // Create and display status dialog box. 
         
            break; 
        case ICSTATUS_STATUS: 
            ProSetBarPos((int) l); // sets status bar positions 
 
        // Watch for abort message 
            while(PeekMessage(&msg, NULL, 0, 0, PM_REMOVE)) 
            { 
                if (msg.message == WM_KEYDOWN && msg.wParam == 
                    VK_ESCAPE) 
                    return 1; 
                if (msg.message == WM_SYSCOMMAND && 
                    (msg.wParam & 0xFFF0) == SC_CLOSE) 
                    return 1; 
 
                TranslateMessage(&msg); 
                DispatchMessage(&msg); 
            } 
            break; 
        case ICSTATUS_END: 
         
        // Close and destroy status dialog box. 
         
            break; 
        case ICSTATUS_YIELD: 
         
         
         
            break; 
    } 
    return 0; 
} 
 
```



 

 




