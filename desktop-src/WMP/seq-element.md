---
title: Seq, элемент
description: Элемент seq содержит элементы, которые определяют статический список воспроизведения или элементы, определяющие интеллектуальный список воспроизведения.
ms.assetid: 849f7b38-25f2-4708-a83c-e651812a1a72
keywords:
- seq, элемент проигрыватель Windows Media
topic_type:
- apiref
api_name:
- seq Element
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b08b3f4dfa448e48f3a9d2472c6ddb46a4d4dfaf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064321"
---
# <a name="seq-element"></a>Seq, элемент

Элемент **Seq** содержит элементы, которые определяют статический список воспроизведения или элементы, определяющие интеллектуальный список воспроизведения.

``` syntax
<seq>
</seq>
```

## <a name="attributes"></a>Атрибуты

Этот элемент не содержит атрибуты.

## <a name="parentchild-elements"></a>Родительские и дочерние элементы



| Иерархия | Элементы                                                               |
|-----------|------------------------------------------------------------------------|
| Parent    | [body](body-element.md)                                               |
| Дочерний     | [носитель](media-element.md), [смартплайлист](smartplaylist-element.md) |



 

## <a name="remarks"></a>Remarks

Если элемент **Seq** содержит только элементы **мультимедиа** , которые ссылаются на определенные элементы мультимедиа, список воспроизведения считается статическим. Если элемент **Seq** содержит элемент **смартплайлист** , он считается динамическим «интеллектуальным» списком воспроизведения.

## <a name="examples"></a>Примеры


```
<seq>
    <media></media>
    <media></media>
</seq>

<seq>
    <smartPlaylist></smartPlaylist>
</seq>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент Body**](body-element.md)
</dt> <dt>

[**Элемент Media**](media-element.md)
</dt> <dt>

[**Смартплайлист, элемент**](smartplaylist-element.md)
</dt> <dt>

[**Windows Справочник по элементам списка воспроизведения мультимедиа**](windows-media-playlist-elements-reference.md)
</dt> </dl>

 

 





