---
title: Сообщение MM_MIXM_LINE_CHANGE (Ммсистем. h)
description: '\_ \_ \_ Устройство микшера отправляет сообщение об изменении строки mm миксм, чтобы уведомить приложение о том, что изменилось состояние звуковой линии на указанном устройстве. Приложение должно обновить отображаемые и кэшированные значения для указанной звуковой строки.'
ms.assetid: 68ada0be-9dc5-4edf-b924-ef0d10a1b79a
keywords:
- сообщение MM_MIXM_LINE_CHANGE Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_MIXM_LINE_CHANGE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 92c4aa10d9934f8cf5f5747ecb4e4eb736af2655
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371178"
---
# <a name="mm_mixm_line_change-message"></a>\_ \_ \_ Сообщение об изменении миксм строки mm

Устройство микшера отправляет сообщение об **\_ \_ \_ изменении строки mm миксм** , чтобы уведомить приложение о том, что изменилось состояние звуковой линии на указанном устройстве. Приложение должно обновить отображаемые и кэшированные значения для указанной звуковой строки.


```C++
MM_MIXM_LINE_CHANGE 
wParam = (WPARAM) hMixer 
lParam = (LPARAM) dwLineID 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hMixer"></span><span id="hmixer"></span><span id="HMIXER"></span>*хмиксер*
</dt> <dd>

Маркер устройства микшера, отправившего сообщение уведомления.

</dd> <dt>

<span id="dwLineID"></span><span id="dwlineid"></span><span id="DWLINEID"></span>*двлинеид*
</dt> <dd>

Идентификатор строки для звуковой строки, которая изменила состояние. Этот идентификатор совпадает с элементом **двлинеид** структуры **миксерлине**, возвращенной функцией **миксержетлинеинфо**.

</dd> </dl>

## <a name="remarks"></a>Remarks

Приложение должно открыть микшерное устройство и указать окно обратного вызова для получения сообщения **об \_ \_ \_ изменении mm миксм Line** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Аудио Миксерс](audio-mixers.md)
</dt> <dt>

[звуковые Mixer сообщения](audio-mixer-messages.md)
</dt> </dl>

 

 





