---
title: Метод Controls. Pause
description: Метод Pause приостанавливает воспроизведение элемента мультимедиа. | Метод Controls. Pause
ms.assetid: 7307a3b2-e5d6-4067-bdb5-38011565142a
keywords:
- приостановить проигрыватель Windows Media метода
- приостановка метода проигрыватель Windows Media, класс controls
- класс элементов управления проигрыватель Windows Media, метод pause
topic_type:
- apiref
api_name:
- Controls.pause
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 898efb51355a1301bc76717f6d0184d0b30d619d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967682"
---
# <a name="controlspause-method"></a>Метод Controls. Pause

Метод **Pause** приостанавливает воспроизведение элемента мультимедиа.

## <a name="syntax"></a>Синтаксис


```JScript
Controls.pause()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

когда файл приостанавливается, проигрыватель Windows Media не предоставляет никаких системных ресурсов, таких как звуковое устройство.

Невозможно приостановить определенные типы носителей, например динамические потоки. Чтобы определить, можно ли приостановить определенный тип носителя, используйте *элементы управления*. **доступно ("Pause")**.

## <a name="examples"></a>Примеры

В следующем примере создается HTML-элемент BUTTON, который использует **Pause** для приостановки воспроизведения. Объект **Player** создан с идентификатором "Player".


```JScript
<INPUT TYPE = "BUTTON"  ID = "PAUSE"  NAME = "PAUSE"  VALUE = "||"
    onClick = "

        /* Check first to be sure the operation is valid. */
        if (Player.controls.isAvailable('Pause'))

            /* Pause the Player. */
            Player.controls.pause();
">
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

[**Элементы управления. доступно**](controls-isavailable.md)
</dt> </dl>

 

 





