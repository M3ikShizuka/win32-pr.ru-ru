---
title: Событие Player. Поситиончанже
description: Событие Поситиончанже возникает при изменении текущей позиции элемента мультимедиа.
ms.assetid: 0561c58c-da5d-438e-adf8-2472405c6b9e
keywords:
- проигрыватель Windows Media событий поситиончанже
- проигрыватель Windows Media событий поситиончанже, класс Player
- класс проигрывателя проигрыватель Windows Media, событие поситиончанже
topic_type:
- apiref
api_name:
- Player.PositionChange
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0156cab32f4a11ec239e7bdfe2b2896a59c44f986f1f1d51b49619e86e6ab4a5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119862404"
---
# <a name="playerpositionchange-event"></a>Событие Player. Поситиончанже

Событие **поситиончанже** возникает при изменении текущей позиции элемента мультимедиа.

## <a name="syntax"></a>Синтаксис


```JScript
Player.PositionChange(
  oldPosition,
  newPosition
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*олдпоситион* 
</dt> <dd>

Число (**Double**), указывающее старую точку.

</dd> <dt>

*невпоситион* 
</dt> <dd>

**Число** (**Double**), задающее новую точку.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Это событие не вызывается во время воспроизведения. Это происходит только тогда, когда что-то активно изменяет текущее положение воспроизводимого мультимедийного элемента, например перемещение маркера поиска или кода, указывающего значение для *элементов управления*. **CurrentPosition**.

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





