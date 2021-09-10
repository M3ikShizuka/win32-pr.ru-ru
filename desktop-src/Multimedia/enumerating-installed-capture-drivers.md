---
title: Перечисление установленных драйверов записи
description: Перечисление установленных драйверов записи
ms.assetid: 3a70bf5b-1e0a-48d3-aa6b-be66692f0400
keywords:
- Функция Капжетдривердескриптион
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 09a053b2de7a69a712914926dbd2ab72be9d1732
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371376"
---
# <a name="enumerating-installed-capture-drivers"></a>Перечисление установленных драйверов записи

В следующем примере функция [**капжетдривердескриптион**](/windows/desktop/api/Vfw/nf-vfw-capgetdriverdescriptiona) используется для получения имен и версий установленных драйверов записи.


```C++
char szDeviceName[80];
char szDeviceVersion[80];

for (wIndex = 0; wIndex < 10; wIndex++) 
{
    if (capGetDriverDescription(
            wIndex, 
            szDeviceName, 
            sizeof (szDeviceName), 
            szDeviceVersion, 
            sizeof (szDeviceVersion)
        )) 
    {
        // Append name to list of installed capture drivers
        // and then let the user select a driver to use.
    }
} 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование видеозаписи](using-video-capture.md)
</dt> </dl>

 

 




