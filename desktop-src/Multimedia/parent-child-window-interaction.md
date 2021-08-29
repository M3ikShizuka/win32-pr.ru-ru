---
title: Взаимодействие с окном Parent-Child
description: Взаимодействие с окном Parent-Child
ms.assetid: de10bf12-4ba4-4c6b-be56-489e4e2b26b1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c6b2ea050fda4cbc6ffc54e318a6a7d01e63db6ace0f1d71e3847f46b68b94ef
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118136753"
---
# <a name="parent-child-window-interaction"></a>Взаимодействие с окном Parent-Child

Некоторые сообщения на уровне системы, такие как [**WM \_ Палеттечанжед**](/windows/desktop/gdi/wm-palettechanged) и [**WM \_ куериневпалетте**](/windows/desktop/gdi/wm-querynewpalette), отправляются только в окна верхнего уровня и перекрывающихся окон. Если окно записи является дочерним окном, его родительский элемент должен пересылать эти сообщения.

Аналогично, если размер родительского окна изменится, может потребоваться отправить сообщения уведомления в окно Capture (захват). И наоборот, при изменении размера записанного видео в окне Capture может потребоваться отправить уведомления родительскому окну. Самый простой способ управления этим — всегда сохранять размеры окна захвата равными размеру захваченного видеопотока, уведомляя родительский элемент при изменении этих измерений.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Windows записи](capture-windows.md)
</dt> </dl>

 

 