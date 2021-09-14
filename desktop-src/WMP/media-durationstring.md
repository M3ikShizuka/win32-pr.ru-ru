---
title: Media. Дуратионстринг
description: Свойство Дуратионстринг извлекает строковое значение, указывающее длительность текущего элемента мультимедиа в формате чч мм СС.
ms.assetid: dfcb4c2e-c62c-4c3e-a9f4-fd147fb5b28c
keywords:
- проигрыватель Windows Media Media. дуратионстринг
topic_type:
- apiref
api_name:
- Media.durationString
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1f1bbb89716ab1d06b176754396611ab22980659
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967498"
---
# <a name="mediadurationstring"></a>Media. Дуратионстринг

Свойство **дуратионстринг** извлекает **строковое** значение, указывающее длительность текущего элемента мультимедиа в формате чч: мм: СС.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *куррентмедиа*. **дуратионстринг**

## <a name="possible-values"></a>Возможные значения

Это свойство является **строкой**, доступная только для чтения.

## <a name="remarks"></a>Комментарии

Если это свойство используется с элементом мультимедиа, отличным от указанного в *проигрывателе*. **куррентмедиа**, он может не содержать допустимое значение. Если размер элемента мультимедиа меньше часа, часть значения чч: в возвращаемом значении не указывается.

Чтобы получить значение этого свойства, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="examples"></a>Примеры

в следующем примере JScript используется *носитель*. **дуратионстринг** , чтобы отобразить длительность текущего элемента мультимедиа в виде форматированного текста. Элемент HTML DIV с именем файла MediaInfo отображает сведения о длительности. Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an event handler to update the display when
 the current media item changes. -->
<SCRIPT LANGUAGE = "JScript"  FOR = Player  EVENT = OpenStateChange(NewState)>

// Test whether the new media item is open.
if (NewState == 13){

   // Write the formatted duration string to the DIV region.
   MediaInfo.innerHTML = "Duration: " + Player.currentMedia.durationString;
}
</SCRIPT>

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

[**Носитель. Длительность**](media-duration.md)
</dt> <dt>

[**Player. Куррентмедиа**](player-currentmedia.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





