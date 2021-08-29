---
title: Атрибут MediaType
description: Атрибут MediaType — это тип содержимого элемента.
ms.assetid: 0d8a6937-32d8-4a4a-87e5-0002f077fefe
keywords:
- проигрыватель Windows Media атрибута MediaType
topic_type:
- apiref
api_name:
- MediaType
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 57f75871e2b258b229483114be8f7673cccb7ca005e0b3618f4cfd803d47fe3f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118996234"
---
# <a name="mediatype-attribute"></a>Атрибут MediaType

Атрибут **mediaType** — это тип содержимого элемента.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)
-   [Другие элементы](other-item-attributes.md)
-   [Элементы фото](photo-item-attributes.md)
-   [Списки воспроизведения](playlist-attributes-ref.md)
-   [Элементы Радио](radio-item-attributes.md)
-   [Элементы видео](video-item-attributes.md)

## <a name="remarks"></a>Remarks

Этот атрибут хранится только в библиотеке.

Этот атрибут имеет одно из следующих значений: "звук", "другое", "Фото", "список воспроизведения", "Радио" или "видео". Используйте этот атрибут с параметром *медиаколлектион*. метод **жетбяттрибуте** для получения списка воспроизведения, содержащего все элементы определенного типа.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> <dt>

[**Медиаколлектион. Жетбяттрибуте**](mediacollection-getbyattribute.md)
</dt> </dl>

 

 





