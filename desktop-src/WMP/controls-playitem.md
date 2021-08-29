---
title: Controls. Плайитем, метод
description: Метод Плайитем воспроизводит указанный элемент мультимедиа. | Controls. Плайитем, метод
ms.assetid: 410e315d-8d5f-4f45-82a7-4249e656c809
keywords:
- проигрыватель Windows Media метода плайитем
- проигрыватель Windows Media метода плайитем, класс controls
- класс элементов управления проигрыватель Windows Media, метод плайитем
topic_type:
- apiref
api_name:
- Controls.playItem
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c6ea371b2e2593ccf9b16d555c60a150ddb6229a2fd884b894d7be41eb61830c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119135727"
---
# <a name="controlsplayitem-method"></a>Controls. Плайитем, метод

Метод **плайитем** воспроизводит указанный элемент мультимедиа.

## <a name="syntax"></a>Синтаксис


```JScript
Controls.playItem(
  theMediaItem
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*семедиаитем* \[ окне\]
</dt> <dd>

Объект **мультимедиа** для воспроизведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

элемент мультимедиа будет загружаться и воспроизводиться автоматически независимо от значения *Параметры*. свойство " **Автозапуск** ". чтобы загрузить элемент без автоматического воспроизведения, задайте *Параметры*. **Автозапуск** в значение false и назначение значения *проигрывателю*. **URL-адрес**, после которого можно вызвать **Воспроизведение** , чтобы начать воспроизведение элемента.

Примечание

**плайитем** работает только с элементами в *куррентплайлист*. Вызов **плайитем** со ссылкой на сохраненный элемент мультимедиа не поддерживается.

## <a name="examples"></a>Примеры

в следующем примере JScript используется **плайитем** для воспроизведения элемента мультимедиа из текущего списка воспроизведения. Элемент для воспроизведения выбирается в зависимости от его позиции в списке воспроизведения. Объект **Player** создан с идентификатором "Player".


```JScript
// Declare a variable to hold the position of the media item 
// in the current playlist. An arbitrary value is supplied here.
var index = 3

// Retrieve the media item at the fourth position in the current playlist.
var media = Player.currentPlaylist.item(index);

// Play the media item.
Player.controls.playItem(media);

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> <dt>

[**Список воспроизведения. элемент**](playlist-item.md)
</dt> </dl>

 

 





