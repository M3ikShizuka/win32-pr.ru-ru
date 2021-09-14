---
title: BUTTONGROUP. Хуешифт
description: Атрибут Хуешифт указывает или получает величину, на которую смещается оттенок изображений BUTTONGROUP.
ms.assetid: 156256ef-ec24-40c4-ad23-064e38c79e69
keywords:
- BUTTONGROUP. хуешифт проигрыватель Windows Media
topic_type:
- apiref
api_name:
- BUTTONGROUP.hueShift
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3bf77faea27ecc5adee6525c4ee8d8ff1541aac4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885349"
---
# <a name="buttongrouphueshift"></a>BUTTONGROUP. Хуешифт

Атрибут **хуешифт** указывает или получает величину, на которую смещается оттенок изображений **BUTTONGROUP** .

``` syntax
        elementID.hueShift
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **числом** для чтения и записи (**float**) со значением в диапазоне от 0,0 до 360,0 со значением по умолчанию 0,0.

## <a name="remarks"></a>Комментарии

Этот атрибут изменяет значение оттенка изображений, заданных атрибутами **дисабледимаже**, **довнимаже**, **ховердовнимаже**, **ховеримаже** и **Image** , если они заданы и ссылаются на 8-битные изображения BMP.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**BUTTONGROUP, элемент**](buttongroup-element.md)
</dt> <dt>

[**BUTTONGROUP. Дисабледимаже**](buttongroup-disabledimage.md)
</dt> <dt>

[**BUTTONGROUP. Довнимаже**](buttongroup-downimage.md)
</dt> <dt>

[**BUTTONGROUP. Ховердовнимаже**](buttongroup-hoverdownimage.md)
</dt> <dt>

[**BUTTONGROUP. Ховеримаже**](buttongroup-hoverimage.md)
</dt> <dt>

[**BUTTONGROUP. Image**](buttongroup-image.md)
</dt> <dt>

[**BUTTONGROUP. насыщенность**](buttongroup-saturation.md)
</dt> </dl>

 

 





