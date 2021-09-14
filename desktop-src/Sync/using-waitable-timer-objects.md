---
description: В следующем примере создается таймер, который будет получать сигнал после 10-секундной задержки.
ms.assetid: 3c84c2ad-6bac-4f14-a633-51d4529314af
title: Использование ожидающих объектов таймера
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 73a23b0d9f6ab74df325be81eb9236bffe6a0c6d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056856"
---
# <a name="using-waitable-timer-objects"></a>Использование ожидающих объектов таймера

В следующем примере создается таймер, который будет получать сигнал после 10-секундной задержки. Во-первых, код использует функцию [**сбой createwaitabletimer**](/windows/win32/api/synchapi/nf-synchapi-createwaitabletimerw) для создания [объекта таймера ожидания](waitable-timer-objects.md). Затем для установки таймера используется функция [**сетваитаблетимер**](/windows/win32/api/synchapi/nf-synchapi-setwaitabletimer) . Код использует функцию [**WaitForSingleObject**](/windows/win32/api/winbase/nf-winbase-registerwaitforsingleobject) для определения момента сигнала таймера.


```C++
#include <windows.h>
#include <stdio.h>

int main()
{
    HANDLE hTimer = NULL;
    LARGE_INTEGER liDueTime;

    liDueTime.QuadPart = -100000000LL;

    // Create an unnamed waitable timer.
    hTimer = CreateWaitableTimer(NULL, TRUE, NULL);
    if (NULL == hTimer)
    {
        printf("CreateWaitableTimer failed (%d)\n", GetLastError());
        return 1;
    }

    printf("Waiting for 10 seconds...\n");

    // Set a timer to wait for 10 seconds.
    if (!SetWaitableTimer(hTimer, &liDueTime, 0, NULL, NULL, 0))
    {
        printf("SetWaitableTimer failed (%d)\n", GetLastError());
        return 2;
    }

    // Wait for the timer.

    if (WaitForSingleObject(hTimer, INFINITE) != WAIT_OBJECT_0)
        printf("WaitForSingleObject failed (%d)\n", GetLastError());
    else printf("Timer was signaled.\n");

    return 0;
}
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование ожидающих таймеров при асинхронном вызове процедуры](using-a-waitable-timer-with-an-asynchronous-procedure-call.md)
</dt> </dl>

 

 
