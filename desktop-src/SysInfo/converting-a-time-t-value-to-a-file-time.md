---
description: Функции времени, включаемые во время выполнения C, используют \_ тип t для представления количества секунд, истекших с полуночи 1 января 1970. В следующем примере значение времени t преобразуется \_ в файловый момент с помощью функции Int32x32To64.
ms.assetid: f626c0b2-a5a1-475d-9a24-64e7b0407278
title: Преобразование значения time_t в файловый момент
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ee866efaed716fb12d2501337236afdb7cf641b9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056854"
---
# <a name="converting-a-time_t-value-to-a-file-time"></a>Преобразование значения времени \_ t в файловый момент

Функции времени, включаемые во время выполнения C, используют \_ тип t для представления количества секунд, истекших с полуночи 1 января 1970. В следующем примере значение времени t преобразуется \_ в файловый момент с помощью функции [**Int32x32To64**](/windows/desktop/api/winnt/nf-winnt-int32x32to64) .


```C++
#include <windows.h>
#include <time.h>

void TimetToFileTime( time_t t, LPFILETIME pft )
{
    LONGLONG ll = Int32x32To64(t, 10000000) + 116444736000000000;
    pft->dwLowDateTime = (DWORD) ll;
    pft->dwHighDateTime = ll >>32;
}
```



После получения времени файла это значение можно преобразовать в системное время с помощью функции [**филетиметосистемтиме**](/windows/win32/api/timezoneapi/nf-timezoneapi-filetimetosystemtime) .

 

 
