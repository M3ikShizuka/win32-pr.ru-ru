---
title: Событие Player. Плайлистколлектионплайлистремовед
description: Событие Плайлистколлектионплайлистремовед возникает при удалении списка воспроизведения из коллекции списков воспроизведения. | Событие Player. Плайлистколлектионплайлистремовед
ms.assetid: 2405be98-b4c2-4b4e-bea6-0c48a3e26f18
keywords:
- проигрыватель Windows Media событий плайлистколлектионплайлистремовед
- проигрыватель Windows Media событий плайлистколлектионплайлистремовед, класс Player
- класс проигрывателя проигрыватель Windows Media, событие плайлистколлектионплайлистремовед
topic_type:
- apiref
api_name:
- Player.PlaylistCollectionPlaylistRemoved
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a449a7b00516f4fee613722d1cc126eb74227948
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056322"
---
# <a name="playerplaylistcollectionplaylistremoved-event"></a>Событие Player. Плайлистколлектионплайлистремовед

Событие **плайлистколлектионплайлистремовед** возникает при удалении списка воспроизведения из коллекции списков воспроизведения.

## <a name="syntax"></a>Синтаксис


```JScript
Player.PlaylistCollectionPlaylistRemoved(
  bstrPlaylistName
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*бстрплайлистнаме* 
</dt> <dd>

**Строка** , указывающая имя списка воспроизведения, который был удален.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Комментарии

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> <dt>

[**Плайлистколлектион. Жетбинаме**](playlistcollection-getbyname.md)
</dt> </dl>

 

 





