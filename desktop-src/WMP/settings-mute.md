---
title: Параметры. без звука
description: Свойство выкл. указывает и получает значение, указывающее, отключено ли звуковое сопровождение.
ms.assetid: d6d4b46d-5631-4af7-bd99-21674f067121
keywords:
- Параметры. отключите проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Settings.mute
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 26c3a6d510f2b5906ea604a783f59b6246ac8b302a2a77d8941237361ee888eb
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120002394"
---
# <a name="settingsmute"></a>Параметры. без звука

Свойство **выкл** . указывает и получает значение, указывающее, отключено ли звуковое сопровождение.

## <a name="syntax"></a>Синтаксис

Player. Settings. выкл.

## <a name="possible-values"></a>Возможные значения

Это свойство является **логическим значением** для чтения и записи.



| Значение | Описание                  |
|-------|------------------------------|
| Да  | Звук отключен.              |
| false | По умолчанию. Звук не отключен. |



 

## <a name="examples"></a>Примеры

В следующем примере создается элемент CHECKBOX HTML, позволяющий пользователю отключить звук и снять с него микрофон. Объект **Player** создан с идентификатором "Player".


```
<!-- Create an HTML CHECKBOX control. -->
<INPUT  TYPE = "CHECKBOX"  ID = MUTE  
             onClick = "
                        /* Use the CHECKBOX state to set 
                           the mute property. */
                        Player.settings.mute = MUTE.checked;
">
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Параметры Объектами**](settings-object.md)
</dt> </dl>

 

 





