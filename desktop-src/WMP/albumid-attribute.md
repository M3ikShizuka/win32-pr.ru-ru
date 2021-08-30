---
title: Атрибут Албумид
description: Атрибут Албумид является уникальным идентификатором для альбома.
ms.assetid: 0412d91a-11a7-434c-8717-a71d85655679
keywords:
- проигрыватель Windows Media атрибута албумид
topic_type:
- apiref
api_name:
- AlbumID
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f2690e4b6dd6bf6c8d795c8a06aca9c65c3f2c17513cf9b8ab8d55419b00d517
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120124074"
---
# <a name="albumid-attribute"></a>Атрибут Албумид

Атрибут **албумид** является уникальным идентификатором для альбома.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)

## <a name="remarks"></a>Remarks

Этот атрибут хранится только в библиотеке.

Уникальный идентификатор представляет собой сочетание названия альбома и имени исполнителя альбома. В этом атрибуте сначала появляется заголовок альбома. При использовании метода [медиаколлектион. жетаттрибутестрингколлектион](mediacollection-getattributestringcollection.md) для получения объекта **StringCollection** с помощью этого атрибута значения сортируются по названию альбома.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Атрибут Албумидалбумартист**](albumidalbumartist-attribute.md)
</dt> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> </dl>

 

 





