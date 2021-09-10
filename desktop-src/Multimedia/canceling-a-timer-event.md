---
title: Отмена события таймера
description: Отмена события таймера
ms.assetid: 4c1be031-e3d5-4d7c-b197-c40c61fc4e2f
keywords:
- Таймеры мультимедиа, события
- таймеры, события
- Функция Тимекиллевент
- Отмена событий таймера
- Таймеры мультимедиа, отмена событий
- таймеры, отмена событий
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1380b2868596e0177e806f5df5217bb839abe61c
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370974"
---
# <a name="canceling-a-timer-event"></a>Отмена события таймера

> [!Note]  
> В этом разделе описывается устаревшая функция. Новые приложения должны использовать функцию [**CreateTimerQueueTimer**](/windows/desktop/api/threadpoollegacyapiset/nf-threadpoollegacyapiset-createtimerqueuetimer) для создания таймеров.

 

Для каждого периодического таймера, создающего вызов [**тимесетевент**](/previous-versions//dd757634(v=vs.85)), приложение должно отменить таймер, вызвав функцию [**тимекиллевент**](/previous-versions//dd757630(v=vs.85)) , прежде чем освободить память, содержащую функцию обратного вызова. Для отмены события таймера может быть вызвана Следующая функция.


```C++
void DestroyTimer(NPSEQ npSeq)
{
    if(npSeq->wTimerID) {                // is timer event pending?
        timeKillEvent(npSeq->wTimerID);  // cancel the event
        npSeq->wTimerID = 0;
    }
} 
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование таймеров мультимедиа](using-multimedia-timers.md)
</dt> </dl>

 

 