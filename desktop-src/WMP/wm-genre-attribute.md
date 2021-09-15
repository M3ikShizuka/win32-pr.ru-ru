---
title: Атрибут WM/жанра
description: Атрибут WM/жанр является жанром содержимого.
ms.assetid: 4b1b0512-d8fd-402a-a5f0-1002c64194f4
keywords:
- проигрыватель Windows Media атрибута WM/жанра
topic_type:
- apiref
api_name:
- WM/Genre
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: aae4a0c6ae27e85fa1ed147a3173c4cc31b20f1b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458650"
---
# <a name="wmgenre-attribute"></a>Атрибут WM/жанра

Атрибут **WM/жанр** является жанром содержимого.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)
-   [Списки воспроизведения компакт-дисков](cd-playlist-attributes.md)
-   [Дорожки компакт-диска](cd-track-attributes.md)
-   [часто используемые Windows атрибуты файла мультимедиа](commonly-used-windows-media-file-attributes.md)
-   [DVD-диски](dvd-attributes.md)
-   [Другие элементы](other-item-attributes.md)
-   [Списки воспроизведения](playlist-attributes-ref.md)
-   [Элементы видео](video-item-attributes.md)

## <a name="remarks"></a>Комментарии

Этот атрибут хранится как в библиотеке (или в кэше), так и в файле цифрового носителя.

Этот атрибут может иметь несколько значений. Чтобы получить все значения атрибута с несколькими значениями, необходимо использовать метод **Media. жетитеминфобитипе** , а не метод **Media. getItemInfo** .

**Жанр** — это псевдоним для этого атрибута.

константа пакета SDK Windows Media Format для этого атрибута — g \_ всзвмженре.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> <dt>

[**Media. Жетитеминфобитипе**](media-getiteminfobytype.md)
</dt> </dl>

 

 





