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
ms.openlocfilehash: 5779552f62007aa3dd3da0e2f4253fcf5499a6be
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347722"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> <dt>

[**Медиаколлектион. Жетбяттрибуте**](mediacollection-getbyattribute.md)
</dt> </dl>

 

 





