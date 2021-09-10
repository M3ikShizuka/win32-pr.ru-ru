---
title: Подключение к драйверу записи
description: Подключение к драйверу записи
ms.assetid: ce83329f-de5a-4428-bc0d-be5f3d35ff1a
keywords:
- макрос Капдривердисконнект
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2161279f5b8b8dc528ee548d0a6a8ad6e9b397f4
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371352"
---
# <a name="connecting-to-a-capture-driver"></a>Подключение к драйверу записи

В следующем примере показано, как подключить окно Capture с помощью обработчика *хвндк* к драйверу мсвидео, а затем отключать их с помощью макроса [**капдривердисконнект**](/windows/desktop/api/Vfw/nf-vfw-capdriverdisconnect) :


```C++
fOK = SendMessage (hWndC, WM_CAP_DRIVER_CONNECT, 0, 0L); 
// 
// Or, use the macro to connect to the MSVIDEO driver: 
// fOK = capDriverConnect(hWndC, 0); 
// 
// Place code to set up and capture video here. 
// 
capDriverDisconnect (hWndC); 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




