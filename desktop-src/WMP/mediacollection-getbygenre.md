---
title: Медиаколлектион. Жетбиженре, метод
description: Метод Жетбиженре извлекает список воспроизведения элементов мультимедиа с указанным жанром.
ms.assetid: 022a0c52-93e1-4ab4-90a7-632bcd6fc004
keywords:
- проигрыватель Windows Media метода жетбиженре
- проигрыватель Windows Media метода жетбиженре, класс медиаколлектион
- класс медиаколлектион проигрыватель Windows Media, метод жетбиженре
topic_type:
- apiref
api_name:
- MediaCollection.getByGenre
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4b73cd7fe9bb3efa9115e2ba5d01b6d12c89898d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967493"
---
# <a name="mediacollectiongetbygenre-method"></a>Медиаколлектион. Жетбиженре, метод

Метод **жетбиженре** извлекает список воспроизведения элементов мультимедиа с указанным жанром.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = MediaCollection.getByGenre(
  genre
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Жанр* \[ окне\]
</dt> <dd>

**Строка** , содержащая название жанра.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает объект **списка воспроизведения** .

## <a name="remarks"></a>Комментарии

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="examples"></a>Примеры

в следующем примере JScript используется *медиаколлектион*. **жетбиженре** для получения списка воспроизведения элементов мультимедиа. Список воспроизведения содержит элементы с жанром, указанным пользователем в HTML-элементе input TEXT с именем GetText. Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Use an HTML BUTTON element to create the playlist and play 
the media items. -->
<INPUT TYPE = "BUTTON"  
       NAME = "PlayGenre"  
       ID = "PlayGenre"  
       VALUE = "Play Genre"

onClick = "
    /* Retrieve the genre text from the user. */
    var genre = GetGenre.value;

    /* Create the playlist using getByGenre. */
    var pl = Player.mediaCollection.getByGenre(genre);

    /* Make the new playlist the current playlist. */
    Player.currentPlaylist = pl;

    /* Play the digital media item in the new playlist. */
    Player.controls.play();
">

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Медиаколлектион**](mediacollection-object.md)
</dt> <dt>

[**Объект списка воспроизведения**](playlist-object.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





