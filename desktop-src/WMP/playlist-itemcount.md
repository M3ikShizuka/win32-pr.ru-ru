---
title: Список воспроизведения. itemCount
description: Атрибут itemCount извлекает количество элементов, отображаемых в данный момент в элементе списка воспроизведения.
ms.assetid: d090d95c-e3c3-41bc-951e-ffeb0a314a0c
keywords:
- проигрыватель Windows Media списка воспроизведения. itemCount
topic_type:
- apiref
api_name:
- PLAYLIST.itemCount
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9b2c831535a0d7ed5643558ddb5305419bab0f0a85b6359f1234f68e78a659ae
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120003004"
---
# <a name="playlistitemcount"></a>Список воспроизведения. itemCount

Атрибут **ItemCount** извлекает количество элементов, отображаемых в данный момент в элементе **списка воспроизведения** .

``` syntax
        elementID.itemCount
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **числом** только для чтения (**длинное целое**).

## <a name="remarks"></a>Remarks

Свойство **ItemCount** будет считать общее число развернутых элементов. Например, если имеется два списка воспроизведения, каждый из которых содержит три элемента мультимедиа, **ItemCount** возвратит 2, если списки воспроизведения не развернуты. Если развернут только первый список воспроизведения, **ItemCount** возвратит 4. Если оба списка воспроизведения развернуты, **ItemCount** возвратит значение 6.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> </dl>

 

 





