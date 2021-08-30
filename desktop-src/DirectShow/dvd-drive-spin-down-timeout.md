---
description: Время ожидания вращения DVD-дисковода
ms.assetid: 2295253d-0199-41b4-95a8-cda049ca93c7
title: Время ожидания вращения DVD-дисковода
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a6283f0846ac374ee9f059b6ac712209ceb0a925b904fcb941b5cf14f0e36d96
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120051884"
---
# <a name="dvd-drive-spin-down-timeout"></a>Время ожидания вращения DVD-дисковода

На переносных компьютерах, чтобы сэкономить время работы батареи, может быть желательно уменьшить продолжительность времени, в течение которого DVD-дисковод будет продолжать работать после приостановки воспроизведения пользователем. По умолчанию на DVD-диске диск вращается в течение двух минут. это значение можно изменить в реестре Windows в этом разделе:


```C++
DWORD HKLM\SOFTWARE\Microsoft\DVDNavigator\DriveSpindown 
[Sec]
```



where


```
Sec
```



время вращения в секундах.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Приложения](appendixes.md)
</dt> </dl>

 

 



