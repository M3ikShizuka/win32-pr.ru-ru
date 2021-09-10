---
title: Получение возможностей драйвера записи
description: Получение возможностей драйвера записи
ms.assetid: 17e90ca6-3646-41cb-8d7a-a2102bc16cc5
keywords:
- Сообщение WM_CAP_DRIVER_GET_CAPS
- макрос Капдривержеткапс
- Структура КАПДРИВЕРКАПС
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6d15a3b1e01ccff738494f287126b7e1ab033056
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371547"
---
# <a name="obtaining-the-capabilities-of-a-capture-driver"></a>Получение возможностей драйвера записи

Сообщение [**о \_ \_ \_ \_ получении политики авторизации устройств WM Cap**](wm-cap-driver-get-caps.md) Возвращает возможности драйвера записи и базового оборудования в структуре [**капдриверкапс**](/windows/win32/api/vfw/ns-vfw-capdrivercaps) . Каждый раз, когда приложение подключается к новому драйверу записи в окне Capture, необходимо обновить структуру **капдриверкапс** . В следующем примере используется макрос [**капдривержеткапс**](/windows/desktop/api/Vfw/nf-vfw-capdrivergetcaps) для получения возможностей драйвера записи.


```C++
CAPDRIVERCAPS CapDrvCaps; 

SendMessage (hWndC, WM_CAP_DRIVER_GET_CAPS, 
    sizeof (CAPDRIVERCAPS), (LONG) (LPVOID) &CapDrvCaps); 

// Or, use the macro to retrieve the driver capabilities. 
// capDriverGetCaps(hWndC, &CapDrvCaps, sizeof (CAPDRIVERCAPS)); 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




