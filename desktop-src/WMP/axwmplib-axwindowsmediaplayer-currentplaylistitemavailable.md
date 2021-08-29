---
title: Событие Куррентплайлиститемаваилабле объекта Аксвиндовсмедиаплайер
description: Событие Куррентплайлиститемаваилабле возникает, когда текущий список воспроизведения станет доступным. | Событие Куррентплайлиститемаваилабле объекта Аксвиндовсмедиаплайер
ms.assetid: 101807c9-b00f-4351-a9a3-5413a52496f4
keywords:
- событие куррентплайлиститемаваилабле объекта аксвиндовсмедиаплайер проигрыватель Windows Media
topic_type:
- apiref
api_name:
- CurrentPlaylistItemAvailable Event of the AxWindowsMediaPlayer Object
api_location:
- AxInterop.WMPLib.dll
api_type:
- Assembly
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e80eac2720d7035d68fa3e94efcaf3205287cd04795a6ccf99c36106d797a8a1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120098784"
---
# <a name="currentplaylistitemavailable-event-of-the-axwindowsmediaplayer-object"></a>Событие Куррентплайлиститемаваилабле объекта Аксвиндовсмедиаплайер

Событие Куррентплайлиститемаваилабле возникает, когда текущий список воспроизведения станет доступным.

``` syntax
[C#]
private void player_CurrentPlaylistItemAvailable(
  object sender,
  _WMPOCXEvents_CurrentPlaylistItemAvailableEvent e
)

[Visual Basic]
Private Sub player_CurrentPlaylistItemAvailable(  
  sender As Object,
  e As _WMPOCXEvents_CurrentPlaylistItemAvailableEvent
) Handles player.CurrentPlaylistItemAvailable
```

## <a name="event-data"></a>Данные о событиях

Обработчик, связанный с этим событием, имеет тип **аксвмплиб. \_ Вмпокксевентс \_ куррентплайлиститемаваилабливенсандлер**. Этот обработчик получает аргумент типа **аксвмплиб. \_ Вмпокксевентс \_ куррентплайлиститемаваилабливент**, который содержит следующее свойство, связанное с этим событием.



| Свойство         | Описание                                                    |
|------------------|----------------------------------------------------------------|
| **бстритемнаме** | Имя System. Стрингсе текущего элемента списка воспроизведения.<br/> |



 

## <a name="remarks"></a>Remarks

Имя текущего списка воспроизведения можно использовать для получения соответствующего интерфейса **ивмпплайлист** из интерфейса ивмпплайлистаррай, возвращаемого методом Ивмпплайлистколлектион. жетбинаме.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------|----------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                          |
| Пространство имен<br/> | **аксвмплиб**<br/>                                                                                                    |
| Сборка<br/>  | <dl> <dt>AxInterop.WMPLib.dll (AxInterop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Аксвиндовсмедиаплайер (VB и C#)**](axwindowsmediaplayer-object--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлист (VB и C#)**](iwmpplaylist--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлистаррай (VB и C#)**](iwmpplaylistarray--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлистколлектион. Жетбинаме (VB и C#)**](wmplibiwmpplaylistcollection-iwmpplaylistcollection-getbyname--vb-and-c.md)
</dt> </dl>

 

 





