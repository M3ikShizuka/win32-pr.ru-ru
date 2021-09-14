---
title: Media. Аттрибутекаунт
description: Свойство Аттрибутекаунт извлекает количество атрибутов, которые могут быть запрошены или заданы для элемента мультимедиа.
ms.assetid: d2a5286f-dde1-48b5-b486-6cee1be463f9
keywords:
- проигрыватель Windows Media Media. аттрибутекаунт
topic_type:
- apiref
api_name:
- Media.attributeCount
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: df4979f670cdd6a79b1b309bc3eceff5a2798223
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967506"
---
# <a name="mediaattributecount"></a>Media. Аттрибутекаунт

Свойство **аттрибутекаунт** извлекает количество атрибутов, которые могут быть запрошены или заданы для элемента мультимедиа.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *куррентмедиа*. **аттрибутекаунт**

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** только для чтения (**длинное целое**).

## <a name="remarks"></a>Комментарии

Чтобы получить значение этого свойства, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

дополнительные сведения об атрибутах, поддерживаемых проигрыватель Windows Media, см. в [справочнике по атрибуту](attribute-reference.md)проигрыватель Windows Media.

**проигрыватель Windows Media 10 Mobile:** Атрибуты для элемента мультимедиа доступны только во время воспроизведения, если они не извлекаются из элемента через коллекцию мультимедиа.

## <a name="examples"></a>Примеры

в следующем примере JScript используется *носитель*. **аттрибутекаунт** для определения количества атрибутов, доступных в текущем элементе мультимедиа. Код использует это значение для печати списка имен и значений атрибутов в текстовой области HTML с именем myText. Объект **Player** создан с идентификатором "Player".


```JScript
// Store the current media object.
var cm = Player.currentMedia;

// Create arrays to hold each attribute name and value.
var atNames = new Array();
var atValues = new Array();

// Loop through the attribute list.   
for(var i = 0; i < cm.attributeCount; i++){

   // Fill the arrays with the attribute info.
   atNames[i] = cm.getAttributeName(i);
   atValues[i] = cm.getItemInfo(atNames[i]);

   // Print the attribute information to the text area.
   myText.value += atNames[i] + ": " + atValues[i];
   myText.value += "\n";
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект мультимедиа**](media-object.md)
</dt> <dt>

[**Media. Жетаттрибутенаме**](media-getattributename.md)
</dt> <dt>

[**Media. getItemInfo**](media-getiteminfo.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





