---
description: Получение буферов
ms.assetid: be61aee9-41d5-42bc-b905-d0216d301faf
title: Получение буферов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ecf516096397eca1fce3a023ee4987d8e8feaa4b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053351"
---
# <a name="getting-buffers"></a>Получение буферов

Если фильтр имеет пользовательский распределитель, использующий ресурсы фильтра, метод [**имемаллокатор::-buffer**](/windows/desktop/api/Strmif/nf-strmif-imemallocator-getbuffer) распределителя должен удерживать блокировку потоковой передачи, как и другие методы потоковой передачи:


```C++
HRESULT CMyInputAllocator::GetBuffer(
    IMediaSample **ppBuffer,
    REFERENCE_TIME *pStartTime, 
    REFERENCE_TIME *pEndTime,
    DWORD dwFlags)
{
    CAutoLock cObjectLock(&m_csReceive);

    /* Use resources. */

    return CMemAllocator::GetBuffer(ppBuffer, pStartTime, pEndTime, dwFlags);    
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Потоки и критические разделы](threads-and-critical-sections.md)
</dt> </dl>

 

 



