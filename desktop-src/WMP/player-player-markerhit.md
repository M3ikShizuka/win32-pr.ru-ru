---
title: Событие Player. Маркерхит
description: Событие Маркерхит возникает при достижении маркера. | Событие Player. Маркерхит
ms.assetid: c97aff61-6f06-4589-a75b-ac2af340cb1d
keywords:
- проигрыватель Windows Media событий маркерхит
- проигрыватель Windows Media событий маркерхит, класс Player
- класс проигрывателя проигрыватель Windows Media, событие маркерхит
topic_type:
- apiref
api_name:
- Player.MarkerHit
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7cce6b9ca7c103e9a9e9151a7ff0467a59786b1e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064445"
---
# <a name="playermarkerhit-event"></a>Событие Player. Маркерхит

Событие **маркерхит** возникает при достижении маркера.

## <a name="syntax"></a>Синтаксис


```JScript
Player.MarkerHit(
  MarkerNum
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*маркернум* 
</dt> <dd>

**Число** (**длинное**), указывающее число попаданий маркера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





