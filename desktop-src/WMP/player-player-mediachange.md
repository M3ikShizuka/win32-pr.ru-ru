---
title: Событие Player. Медиачанже
description: Событие Медиачанже возникает при изменении элемента мультимедиа. | Событие Player. Медиачанже
ms.assetid: c4bdd2ae-c51f-4577-b762-bc84aaf52f76
keywords:
- проигрыватель Windows Media событий медиачанже
- проигрыватель Windows Media событий медиачанже, класс Player
- класс проигрывателя проигрыватель Windows Media, событие медиачанже
topic_type:
- apiref
api_name:
- Player.MediaChange
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 99a63e087356b5d39ae8d751236b8128330c4f3c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064440"
---
# <a name="playermediachange-event"></a>Событие Player. Медиачанже

Событие **медиачанже** возникает при изменении элемента мультимедиа.

## <a name="syntax"></a>Синтаксис


```JScript
Player.MediaChange(
  Item
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Элемент* 
</dt> <dd>

Объект **мультимедиа** , представляющий измененный элемент.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="examples"></a>Примеры

в следующем примере JScript используется элемент HTML DIV с именем MediaName для вывода имени текущего элемента мультимедиа. Код обновляет текст в DIV при каждом возникновении события **медиачанже** . Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an event handler for media change. -->
<SCRIPT FOR = "Player" EVENT = "mediaChange(Item)">
   // Test whether a valid currentMedia object exists.
   if (Player.currentMedia){
      // Display the name of the current media item.
      MediaName.innerHTML = Player.currentMedia.name;
   }
</SCRIPT>

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





