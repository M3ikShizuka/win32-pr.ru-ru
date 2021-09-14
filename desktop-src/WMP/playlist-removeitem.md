---
title: Метод списка воспроизведения. removeItem
description: Метод removeItem удаляет указанный элемент из списка воспроизведения.
ms.assetid: 294ba4fb-967b-4a03-b0c5-6e9c15db3bff
keywords:
- проигрыватель Windows Media метода removeItem
- проигрыватель Windows Media метода removeItem, класс списка воспроизведения
- класс списка воспроизведения проигрыватель Windows Media, метод removeItem
topic_type:
- apiref
api_name:
- Playlist.removeItem
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2de03333e2373744f9e9197be8ed8582997c557d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343227"
---
# <a name="playlistremoveitem-method"></a>Метод списка воспроизведения. removeItem

Метод **RemoveItem** удаляет указанный элемент из списка воспроизведения.

## <a name="syntax"></a>Синтаксис


```JScript
Playlist.removeItem(
  item
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*элемент* \[ окне\]
</dt> <dd>

Объект **мультимедиа** для удаления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Если удаляемый элемент является текущей воспроизводимой записью (*Player*.**Куррентмедиа**), воспроизведение останавливается, а следующий элемент списка воспроизведения переходит в текущий. Если следующий элемент отсутствует, используется предыдущий элемент или, если другие элементы отсутствуют, *проигрыватель*. **куррентмедиа** имеет значение **null**.

Чтобы использовать этот метод, требуется полный доступ к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Player. Куррентмедиа**](player-currentmedia.md)
</dt> <dt>

[**Объект списка воспроизведения**](playlist-object.md)
</dt> <dt>

[**Список воспроизведения. insertItem**](playlist-insertitem.md)
</dt> <dt>

[**Список воспроизведения. элемент**](playlist-item.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





