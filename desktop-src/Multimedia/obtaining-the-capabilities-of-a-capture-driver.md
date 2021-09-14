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
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169627"
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



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




