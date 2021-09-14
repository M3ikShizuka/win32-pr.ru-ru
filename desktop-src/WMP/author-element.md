---
title: AUTHOR, элемент
description: элемент AUTHOR содержит имя автора метафайла мультимедиа Windows или клипа мультимедиа.
ms.assetid: d80aad3d-4471-4310-8d43-2733ed83103c
keywords:
- элемент AUTHOR проигрыватель Windows Media
topic_type:
- apiref
api_name:
- AUTHOR Element
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9d20498ebd7c8a56edc2e32bc2e76422c9b22242
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889856"
---
# <a name="author-element"></a>AUTHOR, элемент

элемент **AUTHOR** содержит имя автора метафайла мультимедиа Windows или клипа мультимедиа.

``` syntax
<AUTHOR>   
   text string
</AUTHOR>
```

## <a name="attributes"></a>Атрибуты

Этот элемент не содержит атрибуты.

## <a name="parentchild-elements"></a>Родительские и дочерние элементы



| Иерархия       | Элемент            |
|-----------------|--------------------|
| Родительские элементы | **ASX**, **запись** |
| Дочерние элементы  | Нет               |



 

## <a name="remarks"></a>Remarks

этот элемент содержит текстовую строку, представляющую имя автора Windowsного метафайла мультимедиа или клипа мультимедиа. Элемент **Author** можно использовать внутри элемента **ASX** и в элементах **entry** .

Если этот элемент отображается в элементе **ASX** , то текст отображается как **Показать** информацию.

Если этот элемент встречается в элементе **entry** , то текст отображается как Автор клипа.

Каждый родительский элемент **ASX** и **entry** должен содержать не более одного дочернего элемента **Author** . Несколько элементов **Author** после первого будут пропущены и не будут отображаться.

## <a name="examples"></a>Примеры


```XML
<ASX VERSION="3.0">
   <AUTHOR>Neal S.</AUTHOR>   <!-- Show author -->
   <ENTRY>
      <REF HREF="mms://example.microsoft.com/clip1.asf" />
      <AUTHOR>Robert P.</AUTHOR>  <!-- Clip author -->
   </ENTRY>
</ASX>

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 70 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Windows Справочник по элементам метафайлов мультимедиа**](windows-media-metafile-elements-reference.md)
</dt> <dt>

[**Windows Ссылка на метафайл мультимедиа**](windows-media-metafile-reference.md)
</dt> </dl>

 

 





