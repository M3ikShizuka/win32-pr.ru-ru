---
title: STARTTIME, элемент
description: элемент STARTTIME определяет индекс времени, на основе которого проигрыватель Windows Media начнет отрисовку потока.
ms.assetid: 9b0199c8-5c95-4b4e-a943-e3bd037bf0bc
keywords:
- элемент STARTTIME проигрыватель Windows Media
topic_type:
- apiref
api_name:
- STARTTIME Element
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 8a882da6c07ec76a94c8e214fe1da11c71680b0c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241732"
---
# <a name="starttime-element"></a>STARTTIME, элемент

элемент **STARTTIME** определяет индекс времени, на основе которого проигрыватель Windows Media начнет отрисовку потока.

``` syntax
<STARTTIME
   VALUE = "hh:mm:ss.fract"
/>
```

## <a name="attributes"></a>Атрибуты

**Значение** (обязательно)

индекс времени (в часах, минутах, секундах и сотых долях секунды), с которого проигрыватель Windows Media начинает воспроизводить поток, определенный в связанном элементе.

## <a name="parentchild-elements"></a>Родительские и дочерние элементы



| Иерархия       | Элементы           |
|-----------------|--------------------|
| Родительские элементы | **entry**, **ref** |
| Дочерние элементы  | None               |



 

## <a name="remarks"></a>Remarks

этот элемент определяет индекс времени в содержимом, где проигрыватель Windows Media — начать отрисовку потока. Этот элемент может использоваться только с сохраненным содержимым по запросу, которое было проиндексировано.

## <a name="examples"></a>Примеры


```XML
<STARTTIME VALUE="1:30.0" />
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 70 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Windows Справочник по элементам метафайлов мультимедиа**](windows-media-metafile-elements-reference.md)
</dt> <dt>

[**Windows Ссылка на метафайл мультимедиа**](windows-media-metafile-reference.md)
</dt> </dl>

 

 





