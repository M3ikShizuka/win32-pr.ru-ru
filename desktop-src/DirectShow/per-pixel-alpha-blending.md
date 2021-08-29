---
description: Per-Pixel альфа-смешение
ms.assetid: 68661dc5-1423-47b2-a0df-858e5eb7f02b
title: Per-Pixel альфа-смешение
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b8722c0483ab4308d2f9d91da7ab94435efc666af5b4353970ff0af54af70532
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119072858"
---
# <a name="per-pixel-alpha-blending"></a>Per-Pixel альфа-смешение

Для многопиксельного альфа-смешения определены четыре подтипа носителей. Эти подтипы поддерживаются, только если VMR находится в режиме смешения. VMR отклоняет соединение, если он не находится в режиме смешения, когда вышестоящий фильтр пытается подключиться с помощью одного из этих подтипов. Эти подтипы определены в UUID. h:

-   МЕДИАСУБТИПЕ \_ ARGB1555
-   МЕДИАСУБТИПЕ \_ ARGB4444
-   МЕДИАСУБТИПЕ \_ ARGB32
-   МЕДИАСУБТИПЕ \_ айув

Дополнительные сведения см. в разделе [несжатые видео подтипы RGB](uncompressed-rgb-video-subtypes.md) и [**подтипы видеороликов YUV**](yuv-video-subtypes.md).

 

 



