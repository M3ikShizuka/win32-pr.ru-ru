---
title: Атрибут Author
description: Атрибут Author — это имя исполнителя или субъекта мультимедиа, связанного с содержимым.
ms.assetid: 6621a955-dd6b-4725-9690-0cc96e73d94f
keywords:
- проигрыватель Windows Media атрибута Author
topic_type:
- apiref
api_name:
- Author
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 28f7bd6acf39142f3947a4df623b4ce2450f3a872386f1f68ec8d7e600b831f2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119864884"
---
# <a name="author-attribute"></a>Атрибут Author

Атрибут **Author** — это имя исполнителя или субъекта мультимедиа, связанного с содержимым.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)
-   [Списки воспроизведения компакт-дисков](cd-playlist-attributes.md)
-   [Дорожки компакт-диска](cd-track-attributes.md)
-   [часто используемые Windows файлы мультимедиа](commonly-used-windows-media-file-attributes.md)
-   [DVD-диски](dvd-attributes.md)
-   [Media. Жетитеминфобитипе](media-getiteminfobytype.md)
-   [Элементы фото](photo-item-attributes.md)
-   [Списки воспроизведения](playlist-attributes-ref.md)
-   [Элементы Радио](radio-item-attributes.md)
-   [Элементы видео](video-item-attributes.md)

## <a name="remarks"></a>Remarks

Этот атрибут хранится как в библиотеке (или в кэше), так и в файле мультимедиа.

Этот атрибут может иметь несколько значений. Чтобы получить все значения атрибута с несколькими значениями, необходимо использовать *носитель*. метод **жетитеминфобитипе** , а не *носитель*. метод **getItemInfo** .

константа пакета SDK Windows Media Format для этого атрибута — g \_ всзвмаусор.

**Субъект** и **исполнитель** — это псевдонимы для этого атрибута.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> </dl>

 

 





