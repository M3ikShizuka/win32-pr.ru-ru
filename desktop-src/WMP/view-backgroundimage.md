---
title: Просмотр. backgroundImage
description: Атрибут backgroundImage указывает или получает фоновое изображение представления или подпредставления.
ms.assetid: 60ffb257-2f43-4ae3-869d-3eb981ef4ae7
keywords:
- просмотр. backgroundImage проигрыватель Windows Media
topic_type:
- apiref
api_name:
- VIEW.backgroundImage
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e96f4a93882e02589d7f15b74ba5cb225f506d69
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064242"
---
# <a name="viewbackgroundimage"></a>Просмотр. backgroundImage

Атрибут **backgroundImage** указывает или получает фоновое изображение **представления** или **подпредставления**.

``` syntax
        elementID.backgroundImage
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **строкой** для чтения и записи.

## <a name="remarks"></a>Remarks

Поддерживаются форматы BMP, JPG, GIF и PNG. Если изображение является 8-битным файлом BMP, его значения тона и насыщенности можно динамически изменить с помощью атрибутов **баккграундимажехуешифт** и **баккграундимажесатуратион** .

в пакете скачивания Windows носителя, если для элемента **представления** задан атрибут **backgroundImage** , необходимо также указать атрибут **backgroundColor** для этого элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**VIEW, элемент**](view-element.md)
</dt> <dt>

[**VIEW. Баккграундимажехуешифт**](view-backgroundimagehueshift.md)
</dt> <dt>

[**VIEW. Баккграундимажесатуратион**](view-backgroundimagesaturation.md)
</dt> </dl>

 

 





