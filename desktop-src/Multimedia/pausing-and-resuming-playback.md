---
title: Приостановка и возобновление воспроизведения
description: Приостановка и возобновление воспроизведения
ms.assetid: f5a7ef22-993c-4aab-bab0-2700289da7a7
keywords:
- Макрос МЦивндпаусе
- Макрос МЦивндресуме
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c1876417b821a57f7ebbac0cd35bec184cc9d2da
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370836"
---
# <a name="pausing-and-resuming-playback"></a>Приостановка и возобновление воспроизведения

Вы можете прервать воспроизведение устройства или файла, связанного с МЦивнд окном, с помощью макроса [**мЦивндпаусе**](/windows/desktop/api/Vfw/nf-vfw-mciwndpause) . Затем можно перезапустить воспроизведение с помощью макроса [**мЦивндресуме**](/windows/desktop/api/Vfw/nf-vfw-mciwndresume) . Если устройство не поддерживает Resume или возникает ошибка, можно использовать макрос [**мЦивндплай**](/windows/desktop/api/Vfw/nf-vfw-mciwndplay) для перезапуска воспроизведения.

В следующем примере создается окно МЦивнд и воспроизводится файл AVI. Команды меню пауза и возобновление доступны пользователю для прерывания и перезапуска воспроизведения.

Стили окон МЦивнд временно изменяются с помощью макроса [**мЦивндчанжестилес**](/windows/desktop/api/Vfw/nf-vfw-mciwndchangestyles) , чтобы запретить отображение диалогового окна ошибки MCI в случае сбоя [**мЦивндресуме**](/windows/desktop/api/Vfw/nf-vfw-mciwndresume) .


```C++
case WM_COMMAND: 
    switch (wParam) 
    { 
        case IDM_CREATEMCIWND:             // creates and plays clip 
            g_hwndMCIWnd = MCIWndCreate(hwnd,  
                g_hinst,                      
                WS_CHILD | WS_VISIBLE |    // standard styles
                MCIWNDF_NOPLAYBAR |        // hides toolbar 
                MCIWNDF_NOTIFYMODE,        // notifies of mode changes
                "sample.avi"); 
 
            MCIWndPlay(g_hwndMCIWnd); 
            break;    
        case IDM_PAUSEMCIWND:              // pauses playback 
            MCIWndPause(g_hwndMCIWnd); 
            MessageBox(hwnd, "MCIWnd", "Pausing Playback", MB_OK); 
            break; 
        case IDM_RESUMEMCIWND:          // resumes playback 
            MCIWndChangeStyles(      // hides error dialog messages
                g_hwndMCIWnd,        // MCIWnd window
                MCIWNDF_NOERRORDLG,  // mask of style to change
                MCIWNDF_NOERRORDLG); // suppresses MCI error dialogs 
 
            lResult = MCIWndResume(g_hwndMCIWnd); 
 
            if(lResult){                   // device doesn't resume 
                MessageBox(hwnd, "MCIWnd", 
                    "Resume with Stop and Play", MB_OK); 
                MCIWndStop(g_hwndMCIWnd); 
                MCIWndPlay(g_hwndMCIWnd); 
 
                MCIWndChangeStyles(        // resumes original styles
                    g_hwndMCIWnd, 
                    MCIWNDF_NOERRORDLG, 
                    NULL); 
        } 
        break; 
    } 
    break; 
 
// Handle other messages here. 
```



 

 




