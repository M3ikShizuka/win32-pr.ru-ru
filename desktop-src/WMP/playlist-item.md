---
title: Метод списка воспроизведения. Item
description: Метод Item извлекает элемент мультимедиа по указанному индексу.
ms.assetid: a564f6db-ede4-4c85-87ca-0e2539d914c2
keywords:
- проигрыватель Windows Media метода элемента
- метод item проигрыватель Windows Media, класс списка воспроизведения
- класс списка воспроизведения проигрыватель Windows Media, метод элемента
topic_type:
- apiref
api_name:
- Playlist.item
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 79c69386871aeec33dbc36a066ce3f75e80d7514
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458419"
---
# <a name="playlistitem-method"></a>Метод списка воспроизведения. Item

Метод **Item** извлекает элемент мультимедиа по указанному индексу.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = Playlist.item(
  index
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*индекс* \[ окне\]
</dt> <dd>

**Число** (**Long**), содержащее индекс извлекаемого элемента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает объект **мультимедиа** .

## <a name="remarks"></a>Remarks

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="examples"></a>Примеры

в следующем примере JScript используется *список воспроизведения*. **элемент** для извлечения элемента мультимедиа из текущего списка воспроизведения на основе выбора пользователя. Был создан HTML-элемент SELECT с именем "список", который заполняется заголовками из текущего списка воспроизведения. Объект **Player** создан с идентификатором "Player".


```JScript
// Store the value of the selected item in the list box
// using the selectedIndex property.
var index = weblist.selectedIndex;

// Store the corresponding digital media object from the current playlist.
var listItem = Player.currentPlaylist.item(index);

// Set the URL using the listItem variable.
Player.URL = listItem.sourceURL;

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

[**Объект списка воспроизведения**](playlist-object.md)
</dt> <dt>

[**Список воспроизведения. insertItem**](playlist-insertitem.md)
</dt> <dt>

[**Список воспроизведения. removeItem**](playlist-removeitem.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





