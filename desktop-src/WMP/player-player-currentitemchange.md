---
title: Событие Player. Куррентитемчанже
description: Событие Куррентитемчанже возникает при изменении Controls. currentItem.
ms.assetid: e6f68aeb-d7e7-460b-adc9-647f28c678a1
keywords:
- проигрыватель Windows Media событий куррентитемчанже
- проигрыватель Windows Media событий куррентитемчанже, класс Player
- класс проигрывателя проигрыватель Windows Media, событие куррентитемчанже
topic_type:
- apiref
api_name:
- Player.CurrentItemChange
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e4c425184bf4b338177ec892ed5362c085dd8cb7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064464"
---
# <a name="playercurrentitemchange-event"></a>Событие Player. Куррентитемчанже

Событие **куррентитемчанже** возникает при использовании *элементов управления*. **currentItem** изменения.

## <a name="syntax"></a>Синтаксис


```JScript
Player.CurrentItemChange()
```



## <a name="parameters"></a>Параметры

У этого события нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="examples"></a>Примеры

в следующем примере JScript демонстрируется обработчик событий для *проигрывателя*. событие **куррентитемчанже** . Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an HTML text box to display the media item name. -->
<INPUT TYPE="TEXT" NAME="MEDIA">

<!-- Create an event handler. -->
<SCRIPT LANGUAGE = "JScript"  FOR = Player EVENT = currentItemChange()>

   // Display the name of the new media item.
   MEDIA.value = Player.currentMedia.name;

</SCRIPT>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Controls. currentItem**](controls-currentitem.md)
</dt> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





