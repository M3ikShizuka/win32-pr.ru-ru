---
title: Атрибут WM/Language
description: Атрибут WM/Language является языком элемента.
ms.assetid: aebfb518-61ca-4b75-875a-ce2127a74b67
keywords:
- проигрыватель Windows Media атрибута WM/Language
topic_type:
- apiref
api_name:
- WM/Language
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 172cc8498bf5360e29822a484bcc2ddacd70b8b7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458647"
---
# <a name="wmlanguage-attribute"></a>Атрибут WM/Language

Атрибут **WM/Language** является языком элемента.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)
-   [часто используемые Windows атрибуты файла мультимедиа](commonly-used-windows-media-file-attributes.md)
-   [Элементы Радио](radio-item-attributes.md)
-   [Элементы видео](video-item-attributes.md)

## <a name="remarks"></a>Комментарии

Этот атрибут хранится как в библиотеке, так и в файле цифрового мультимедиа.

Этот атрибут может иметь несколько значений. Чтобы получить все значения атрибута с несколькими значениями, необходимо использовать метод **Media. жетитеминфобитипе** , а не метод **Media. getItemInfo** .

**Язык** является псевдонимом для этого атрибута.

константа пакета SDK Windows Media Format для этого атрибута — g \_ всзвмлангуаже.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 series или более поздней версии (элемент radio поддерживается только в серии проигрыватель Windows Media 9)<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> <dt>

[**Media. Жетитеминфобитипе**](media-getiteminfobytype.md)
</dt> </dl>

 

 





