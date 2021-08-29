---
title: Ручная запись кадров
description: Ручная запись кадров
ms.assetid: 7c5576ff-2694-4f44-a386-03bbc6f9c2ed
keywords:
- Сообщение WM_CAP_SINGLE_FRAME_OPEN
- Сообщение WM_CAP_SINGLE_FRAME
- Сообщение WM_CAP_SINGLE_FRAME_CLOSE
- макрос Капкаптуресинглефрамеопен
- макрос Капкаптуресинглефраме
- макрос Капкаптуресинглефрамеклосе
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3e9024f8759697248b1aadf2f46f902c4bf706c9d10417281d9b5c4f61fc1e94
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118138859"
---
# <a name="manual-frame-capture"></a>Ручная запись кадров

Если вы хотите отдельно указать кадры для записи в видеопотоке, вы можете управлять этой последовательностью, используя [**\_ \_ \_ \_ открытые фреймы WM Cap**](wm-cap-single-frame-open.md), [**\_ \_ одинарный \_ фрейм**](wm-cap-single-frame.md)с ограничением WM, а также [**\_ \_ \_ \_ закрывать отдельные фреймы**](wm-cap-single-frame-close.md) (или макросы [**капкаптуресинглефрамеопен**](/windows/desktop/api/Vfw/nf-vfw-capcapturesingleframeopen), [**капкаптуресинглефраме**](/windows/desktop/api/Vfw/nf-vfw-capcapturesingleframe)и [**капкаптуресинглефрамеклосе**](/windows/desktop/api/Vfw/nf-vfw-capcapturesingleframeclose) ). Как правило, эти сообщения используются для создания анимации путем добавления отдельных кадров в файл записи. \_ \_ При открытии одиночного кадра WM Cap \_ \_ открывается файл для операции записи, управляемой вручную. \_ \_ Один кадр крепления WM \_ фиксирует отдельный кадр и добавляет его в файл записи. \_ \_ \_ При закрытии одиночного кадра WM Cap \_ закрывается файл, используемый для ручного захвата кадров.

> [!Note]  
> Этот метод отслеживания не поддерживает одновременную запись звука с захватом видео.

 

 

 




