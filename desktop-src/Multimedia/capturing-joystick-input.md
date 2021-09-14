---
title: Запись входных данных джойстика
description: Запись входных данных джойстика
ms.assetid: 1214fe5a-5a6a-4c6c-9b77-94eeb73f60da
keywords:
- Джойстики, запись входных данных
- запись входных данных джойстика
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b23fd3717ad09fd2e52f1a815f7d13b91963a13e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272360"
---
# <a name="capturing-joystick-input"></a>Запись входных данных джойстика

Большая часть кода, управляющего джойстиком, находится в главной функции окна. В следующей части обработчика сообщений приложение вызывает [**жойсеткаптуре**](/windows/win32/api/joystickapi/nf-joystickapi-joysetcapture) для записи входных данных из джойстика JOYSTICKID1.


```C++
case WM_CREATE: 
    if(joySetCapture(hWnd, JOYSTICKID1, NULL, FALSE)) 
    { 
        MessageBeep(MB_ICONEXCLAMATION); 
        MessageBox(hWnd, "Couldn't capture the joystick.", NULL, 
            MB_OK | MB_ICONEXCLAMATION); 
        PostMessage(hWnd,WM_CLOSE,0,0L); 
    } 
    break; 
 
```



 

 