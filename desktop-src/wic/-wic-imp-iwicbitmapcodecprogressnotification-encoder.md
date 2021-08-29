---
description: Реализация Ивикбитмапкодекпрогресснотификатион (кодировщик)
ms.assetid: d470ec93-d329-48c0-9556-0c15daece491
title: Реализация Ивикбитмапкодекпрогресснотификатион (кодировщик)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 79c4f7df833fece592fa6c536e32cff4d4e0505c11a7acdf153c80fa343ccacb
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118965033"
---
# <a name="implementing-iwicbitmapcodecprogressnotification-encoder"></a>Реализация Ивикбитмапкодекпрогресснотификатион (кодировщик)

## <a name="iwicbitmapcodecprogressnotification"></a>ивикбитмапкодекпрогресснотификатион

Хотя интерфейс [**ивикбитмапкодекпрогресснотификатион**](/windows/desktop/api/Wincodec/nn-wincodec-iwicbitmapcodecprogressnotification) является необязательным, рекомендуется реализовать его в классе кодировщика уровня контейнера. Этот интерфейс рассматривается более подробно в разделе [Реализация ивикбитмапкодекпрогресснотификатион (декодер)](-wic-imp-iwicbitmapcodecprogressnotification-decoder.md). Реализация одинакова для декодера и кодировщика.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Зрения**
</dt> <dt>

[Реализация Ивикбитмапенкодер](-wic-imp-iwicbitmapencoder.md)
</dt> <dt>

[Реализация Ивикбитмапфраминкоде](-wic-imp-iwicbitmapframeencode.md)
</dt> <dt>

[Написание WIC-Enabled КОДЕка](-wic-howtowriteacodec.md)
</dt> <dt>

[Windows Общие сведения о компонентах обработки изображений](-wic-about-windows-imaging-codec.md)
</dt> <dt>

[Реализация Ивикбитмапкодекпрогресснотификатион (декодер)](-wic-imp-iwicbitmapcodecprogressnotification-decoder.md)
</dt> </dl>

 

 



