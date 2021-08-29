---
description: В следующем примере кода открывается последовательный порт для перекрывающихся операций ввода-вывода, создается маска событий для мониторинга сигналов CTS и DSR, а затем ожидается возникновение события.
ms.assetid: 23ebcb04-1571-4e93-a549-46ad6b9d4272
title: Мониторинг событий связи
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7f9e3cb28e251450d5302227cbeaf9fa6aac6c8734ea0646757ac2b4291c8ff3
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120131644"
---
# <a name="monitoring-communications-events"></a>Мониторинг событий связи

В следующем примере кода открывается последовательный порт для перекрывающихся операций ввода-вывода, создается маска событий для мониторинга сигналов CTS и DSR, а затем ожидается возникновение события. Функция [**ваиткоммевент**](/windows/desktop/api/Winbase/nf-winbase-waitcommevent) должна выполняться как перекрывающаяся операция, чтобы другие потоки процесса могли выполнять операции ввода-вывода в течение ожидания.


```C++
#include <windows.h>
#include <tchar.h>
#include <assert.h>
#include <stdio.h>

void _tmain(
            int argc, 
            TCHAR *argv[]
           )
{
    HANDLE hCom;
    OVERLAPPED o;
    BOOL fSuccess;
    DWORD dwEvtMask;

    hCom = CreateFile( TEXT("\\\\.\\COM1"),
        GENERIC_READ | GENERIC_WRITE,
        0,    // exclusive access 
        NULL, // default security attributes 
        OPEN_EXISTING,
        FILE_FLAG_OVERLAPPED,
        NULL 
        );

    if (hCom == INVALID_HANDLE_VALUE) 
    {
        // Handle the error. 
        printf("CreateFile failed with error %d.\n", GetLastError());
        return;
    }

    // Set the event mask. 

    fSuccess = SetCommMask(hCom, EV_CTS | EV_DSR);

    if (!fSuccess) 
    {
        // Handle the error. 
        printf("SetCommMask failed with error %d.\n", GetLastError());
        return;
    }

    // Create an event object for use by WaitCommEvent. 

    o.hEvent = CreateEvent(
        NULL,   // default security attributes 
        TRUE,   // manual-reset event 
        FALSE,  // not signaled 
        NULL    // no name
         );
    

    // Initialize the rest of the OVERLAPPED structure to zero.
    o.Internal = 0;
    o.InternalHigh = 0;
    o.Offset = 0;
    o.OffsetHigh = 0;

    assert(o.hEvent);

    if (WaitCommEvent(hCom, &dwEvtMask, &o)) 
    {
        if (dwEvtMask & EV_DSR) 
        {
             // To do.
        }

        if (dwEvtMask & EV_CTS) 
        {
            // To do. 
        }
    }
    else
    {
        DWORD dwRet = GetLastError();
        if( ERROR_IO_PENDING == dwRet)
        {
            printf("I/O is pending...\n");

            // To do.
        }
        else 
            printf("Wait failed with error %d.\n", GetLastError());
    }
}
```



 

 



