---
title: Закрытие всех устройств MCI, используемых приложением
description: Закрытие всех устройств MCI, используемых приложением
ms.assetid: 1d7d3800-b38f-4187-ba57-9849fef4d707
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b84db0bc6a6160098a3714f9cc7dbf455427bc28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057523"
---
# <a name="closing-all-mci-devices-used-by-an-application"></a>Закрытие всех устройств MCI, используемых приложением

В следующем примере закрываются все устройства MCI, открытые приложением с помощью функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) .


```C++
UINT wDeviceID;
DWORD dwReturn;
 
// Closes all MCI devices opened by this application.
// Waits until devices are closed before returning.

if(dwReturn = mciSendCommand(MCI_ALL_DEVICE_ID, MCI_CLOSE, MCI_WAIT, 
    NULL))
    
    // Error, unable to close all devices.
    
```



 

 