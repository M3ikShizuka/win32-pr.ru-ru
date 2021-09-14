---
title: Controls. currentPosition
description: Свойство currentPosition указывает или получает текущую позицию в элементе мультимедиа за считаные секунды с начала.
ms.assetid: 374ad144-3f74-4d1b-bec5-1cd0f03777b7
keywords:
- controls. currentPosition проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Controls.currentPosition
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 12c690c102bb95c1a58785f18d727ffdae2a82c4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967710"
---
# <a name="controlscurrentposition"></a>Controls. currentPosition

Свойство **CurrentPosition** указывает или получает текущую позицию в элементе мультимедиа за считаные секунды с начала.

``` syntax
player.controls.currentPosition
      
```

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** для чтения и записи (**Double**).

## <a name="examples"></a>Примеры

В следующем примере **CurrentPosition** используется для поиска расположения, предоставленного пользователем. для выполнения кода JScript создается HTML-элемент BUTTON. Элемент ввода текста HTML с именем setPosition был создан для принятия значения в секундах от пользователя. Объект **Player** создан с идентификатором "Player".


```JScript
<INPUT TYPE = "BUTTON"  ID = "Set"  NAME = "Set"  VALUE = "Set Position"

    /* Check to be sure the TEXT element contains a valid value. */
    if (!isNaN(setPosition.value) && (setPosition.value != '))

    /* Set the current position when the user clicks the button. */
    onClick = "Player.controls.currentPosition = setPosition.value;
">
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> </dl>

 

 





