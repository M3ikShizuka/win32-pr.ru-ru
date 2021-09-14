---
title: Отправка команды
description: Отправка команды
ms.assetid: 28c38f36-b6a7-44da-95e2-25b3dccefc84
keywords:
- Функция mciSendString
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e69536b167b8fde648c3f3743058542d74bd8647
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173608"
---
# <a name="sending-a-command"></a>Отправка команды

Следующий пример функции отправляет команду [**Play**](play.md) с флагами "from" и "to" с помощью функции [**mciSendString**](/previous-versions//dd757161(v=vs.85)) .


```C++
BOOL PlayFromTo(LPTSTR lpstrAlias, DWORD dwFrom, DWORD dwTo) 
{ 
    TCHAR achCommandBuff[128]; 
    int result;
    MCIERROR err;

    // Form the command string.
    result = _stprintf_s(
        achCommandBuff, 
        TEXT("play %s from %u to %u"), 
        lpstrAlias, dwFrom, dwTo); 

    if (result == -1)
    {
        return FALSE;
    }

    // Send the command string.
    err = mciSendString(achCommandBuff, NULL, 0, NULL); 
    if (err != 0)
    {
        return FALSE;
    }

    return TRUE;
} 
```



 

 