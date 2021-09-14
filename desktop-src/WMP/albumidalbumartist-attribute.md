---
title: Атрибут Албумидалбумартист
description: Атрибут Албумидалбумартист является уникальным идентификатором для альбома.
ms.assetid: beaa8d01-1722-4545-8705-6b3d130113b1
keywords:
- проигрыватель Windows Media атрибута албумидалбумартист
topic_type:
- apiref
api_name:
- AlbumIDAlbumArtist
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1925f40a50b15efcd339ad949d5d54ddb915cbe9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890120"
---
# <a name="albumidalbumartist-attribute"></a>Атрибут Албумидалбумартист

Атрибут **албумидалбумартист** является уникальным идентификатором для альбома.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)

## <a name="remarks"></a>Комментарии

Этот атрибут хранится только в библиотеке.

Уникальный идентификатор представляет собой сочетание названия альбома и имени исполнителя альбома. В этом атрибуте сначала появляется имя исполнителя альбома. При использовании метода [медиаколлектион. жетаттрибутестрингколлектион](mediacollection-getattributestringcollection.md) для получения объекта **StringCollection** с помощью этого атрибута значения сортируются по имени исполнителя альбома.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Атрибут Албумид**](albumid-attribute.md)
</dt> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> </dl>

 

 





