---
title: сикслидер
description: Это Стандартный ПОЛЗУНок со следующими значениями по умолчанию. | сикслидер
ms.assetid: 9fdb0f70-e5ce-4dbc-aeba-44fa0e2c9b3c
keywords:
- сикслидер проигрыватель Windows Media
topic_type:
- apiref
api_name:
- SEEKSLIDER
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 59808fa7c41acfcc28b715362b8724c7f113faee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064330"
---
# <a name="seekslider"></a>сикслидер

Это Стандартный **ползунок** со следующими значениями по умолчанию.

``` syntax
toolTip="Seek"
foregroundProgress="wmpprop:player.network.downloadProgress"
max="wmpprop:player.currentMedia.duration"
min="0"
value="wmpprop:player.controls.currentPosition"
onDragEnd="jscript:player.controls.currentPosition=value;"
useForegroundProgress="true"
```

## <a name="remarks"></a>Remarks

При этом создается элемент управления " **ползунок** ", который ищет файл мультимедиа в любое положение. Всплывающие подсказки локализованы. Все свойства этого **ползунка** можно переопределить, явно указав их.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 7,0 или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент SLIDER**](slider-element.md)
</dt> </dl>

 

 





