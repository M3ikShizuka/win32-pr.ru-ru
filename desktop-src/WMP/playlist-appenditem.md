---
title: Метод списка воспроизведения. Аппендитем
description: Метод Аппендитем добавляет элемент мультимедиа в конец списка воспроизведения.
ms.assetid: cc956491-7936-49e7-90ca-1f71e03448cd
keywords:
- проигрыватель Windows Media метода аппендитем
- проигрыватель Windows Media метода аппендитем, класс списка воспроизведения
- класс списка воспроизведения проигрыватель Windows Media, метод аппендитем
topic_type:
- apiref
api_name:
- Playlist.appendItem
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 828799d5b6e71e7ff0e7be4c1e55714f6343be51
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343326"
---
# <a name="playlistappenditem-method"></a>Метод списка воспроизведения. Аппендитем

Метод **аппендитем** добавляет элемент мультимедиа в конец списка воспроизведения.

## <a name="syntax"></a>Синтаксис


```JScript
Playlist.appendItem(
  item
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*элемент* \[ окне\]
</dt> <dd>

Добавляемый объект **мультимедиа** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Чтобы использовать этот метод, требуется полный доступ к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="examples"></a>Примеры

в следующем примере JScript используется *список воспроизведения*. **аппендитем** добавить текущий элемент мультимедиа в список воспроизведения с именем "срилист". Объект **Player** создан с идентификатором "Player".


```JScript
// Get the current media item.
var currMedia = Player.currentMedia;

// Get the playlist object by name.
var plThreeList = Player.playlistCollection.getByName("ThreeList").item(0);

// Append the media item to the playlist.
plThreeList.appendItem(currMedia);

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект списка воспроизведения**](playlist-object.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





