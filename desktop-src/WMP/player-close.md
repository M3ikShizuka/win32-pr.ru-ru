---
title: Метод Player. Close
description: метод close освобождает проигрыватель Windows Media ресурсы.
ms.assetid: 15bd5a05-dbfa-4bea-90c2-afd9f69631e0
keywords:
- метод close проигрыватель Windows Media
- метод close проигрыватель Windows Media, класс Player
- класс Player проигрыватель Windows Media, метод close
topic_type:
- apiref
api_name:
- Player.close
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: debc2667c42da92b3a2639e0f14c767d2b5b0651
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242461"
---
# <a name="playerclose-method"></a>Метод Player. Close

метод **close** освобождает проигрыватель Windows Media ресурсы.

## <a name="syntax"></a>Синтаксис


```JScript
Player.close()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

этот метод закрывает текущий файл мультимедиа, но не проигрыватель Windows Media самого себя.

## <a name="examples"></a>Примеры

в следующем примере создается HTML-элемент BUTTON, который при щелчке останавливает воспроизведение в проигрыватель Windows Media и освобождает используемые ресурсы. Объект **Player** создан с идентификатором "Player".


```JScript
<INPUT  TYPE = "BUTTON"  ID = "CLOSEIT"  VALUE = "Close it"  onClick = "

        /* Close the Player object. */
        Player.close();
">

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

 

 





