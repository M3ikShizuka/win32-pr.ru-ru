---
title: Носитель. Длительность
description: Свойство Duration извлекает продолжительность текущего элемента мультимедиа за считанные секунды.
ms.assetid: d7d36858-812d-471b-84ce-fe2ab96b86b3
keywords:
- проигрыватель Windows Media мультимедиа. длительность
topic_type:
- apiref
api_name:
- Media.duration
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 71586f6aa37401d56a9e9537bfbea6c5af23f318
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967505"
---
# <a name="mediaduration"></a>Носитель. Длительность

Свойство **Duration** извлекает продолжительность текущего элемента мультимедиа за считанные секунды.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *куррентмедиа*. **Длительность**

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** только для чтения ( **Double**).

## <a name="remarks"></a>Комментарии

Если это свойство используется с элементом мультимедиа, отличным от указанного в *проигрывателе*. **куррентмедиа**, он может не содержать допустимое значение.

чтобы получить длительность для файлов, которые не находятся в библиотеке пользователя, необходимо подождать, пока проигрыватель Windows Media откроет файл. то есть текущий Опенстате должен равняться Медиаопен. Это можно проверить, обрабатывая *проигрыватель*. Событие **опенстатечанже** или путем периодической проверки значения *игрока*. **опенстате**.

Для списков воспроизведения продолжительность каждого элемента мультимедиа может быть получена при открытии отдельного элемента мультимедиа, а не при открытии списка воспроизведения.

Чтобы получить значение этого свойства, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

в следующем примере JScript используется *носитель*. **Длительность** для показа времени, оставшегося в текущем элементе мультимедиа. В элементе HTML DIV с именем Ремтиме отображаются сведения. Таймер HTML обновляет текст в элементе DIV каждую секунду.

следующий код JScript запускает таймер:


```JScript
// Execute the update() function at one-second intervals.
idTmr = window.setInterval("update()",1000);
```



следующий код JScript останавливает таймер:


```JScript
window.clearInterval(idTmr);
```



Используйте *проигрыватель*. Событие **плайстатечанже** с инструкцией **switch** , чтобы определить время запуска и завершения таймера.

следующий JScript код выполняется каждый раз, когда таймер вызывает функцию update:


```JScript
// Store the current position of the current media item.
var TimeNow = Player.controls.currentPosition;

// Display the time remaining information.
RemTime.innerHTML = "Seconds remaining: ";

// Subtract the current position from the duration of the current media.
// Use the Math.floor method to round the result down to the nearest integer.
RemTime.innerHTML += Math.floor(Player.currentMedia.duration - TimeNow);
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

[**Player. Куррентмедиа**](player-currentmedia.md)
</dt> <dt>

[**Событие Player. Плайстатечанже**](player-player-playstatechange.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





