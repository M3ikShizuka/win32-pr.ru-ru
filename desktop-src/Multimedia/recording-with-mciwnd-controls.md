---
title: Запись с помощью элементов управления МЦивнд
description: Запись с помощью элементов управления МЦивнд
ms.assetid: 65a57400-aeea-4a27-8d51-37d3d9e9bd55
keywords:
- Функция МЦивндкреате
- Макрос МЦивнднев
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 814bd9f92b895c03ccbb073f830dbf31dcd2e3c2
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370848"
---
# <a name="recording-with-mciwnd-controls"></a>Запись с помощью элементов управления МЦивнд

В следующем примере записывается звук звукозаписи с помощью встроенных элементов управления окна МЦивнд. В примере создается окно МЦивнд с помощью \_ стиля окна записи мЦивндф с функцией [**мЦивндкреате**](/windows/desktop/api/Vfw/nf-vfw-mciwndcreatea) для добавления кнопки **записи** на панель инструментов. Макрос [**мЦивнднев**](/windows/desktop/api/Vfw/nf-vfw-mciwndnew) указывает, что новый файл связан с окном мЦивнд и что устройство аудио аудио будет предоставлять свое содержимое. Вторая команда меню, IDM \_ савемЦивнд, позволяет пользователю сохранить запись и выбрать имя файла с помощью макроса [**мЦивндсаведиалог**](/windows/desktop/api/Vfw/nf-vfw-mciwndsavedialog) .


```C++
case WM_COMMAND: 
    switch (wParam) { 
    case IDM_CREATEMCIWND: 
        g_hwndMCIWnd = MCIWndCreate(hwnd, g_hinst, 
            WS_VISIBLE | MCIWNDF_RECORD, NULL); 
        MCIWndNew(g_hwndMCIWnd, "waveaudio"); 
        break;    
    case IDM_SAVEMCIWND: 
        MCIWndSaveDialog(g_hwndMCIWnd); 
        break; 
    } 
```



 

 




