---
title: БУТТОНЕЛЕМЕНТ. Маппингколор
description: Атрибут Маппингколор указывает или получает ключ цвета, определяющий этот БУТТОНЕЛЕМЕНТ в BUTTONGROUP.
ms.assetid: e7b1663c-3263-41d5-9a69-4cf1dcf0fc1f
keywords:
- буттонелемент. маппингколор проигрыватель Windows Media
topic_type:
- apiref
api_name:
- BUTTONELEMENT.mappingColor
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7318f01246578fe8ff34118427c95afb7b3bb098
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889312"
---
# <a name="buttonelementmappingcolor"></a>БУТТОНЕЛЕМЕНТ. Маппингколор

Атрибут **маппингколор** указывает или получает ключ цвета, определяющий этот **буттонелемент** в **BUTTONGROUP**.

``` syntax
        elementID.mappingColor
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **строкой** для чтения и записи, содержащей любое значение цвета Microsoft Internet Explorer. У него нет значения по умолчанию.

## <a name="remarks"></a>Комментарии

Этот атрибут определяет цвет области в группе кнопок **маппингимаже** , которая соответствует этому элементу Button. Все щелчки в этом регионе обрабатываются этим элементом кнопки.

Если указан недопустимый цвет, **буттонелемент** не активируется.

## <a name="examples"></a>Примеры

Следующий пример представляет собой полный файл определения обложки, иллюстрирующий использование некоторых атрибутов **буттонелемент** . Его можно найти в каталоге Samples, который был установлен вместе с пакетом SDK.


```
<THEME>
  <VIEW
    backgroundImage = "background.bmp"
    titleBar = "False"
  >
    <PLAYER
      URL = "https://proseware.com/mellow.wma"
    />
    <EFFECTS
      id = "myeffects"
      top = "25"
      left = "88"
      width = "180"
      height = "150"
    />
    <BUTTONGROUP
      mappingImage = "map.bmp"
      hoverImage = "hover.bmp"
    >
      <BUTTONELEMENT
        mappingColor = "#00FF00"
        upToolTip = "Next"
        onClick = "JScript:myeffects.next();"
      />
      <BUTTONELEMENT
        mappingColor = "#FF0000"
        upToolTip = "Previous"
        onClick = "JScript:myeffects.previous();"
      />
    </BUTTONGROUP>
  </VIEW>
</THEME>

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на цвет**](color-reference.md)
</dt> <dt>

[**БУТТОНЕЛЕМЕНТ, элемент**](buttonelement-element.md)
</dt> <dt>

[**BUTTONGROUP. Маппингимаже**](buttongroup-mappingimage.md)
</dt> </dl>

 

 





