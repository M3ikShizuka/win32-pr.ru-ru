---
title: Определение того, может ли драйвер управлять входным форматом
description: Определение того, может ли драйвер управлять входным форматом
ms.assetid: 456eab43-d830-4a28-b724-3ef35b852372
keywords:
- Диспетчер сжатия видео (ВКМ), формат ввода
- ВКМ (диспетчер сжатия видео), формат ввода
- Макрос Икдравкуери
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 07b3e2da69f8c061a7d0aefe847f40113d5104d8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067712"
---
# <a name="determining-if-a-driver-can-handle-the-input-format"></a>Определение того, может ли драйвер управлять входным форматом

В следующем примере показано, как проверить формат ввода с помощью макроса [**икдравкуери**](/windows/desktop/api/Vfw/nf-vfw-icdrawquery) .


```C++
// lpbiIn points to BITMAPINFOHEADER structure indicating the input 
// format. 

if (ICDrawQuery(hIC, lpbiIn) == ICERR_OK) 
{ 
    // Driver recognizes the input format. 
} 
else 
{ 
    // Need a different decompressor. 
} 
 
```



 

 




