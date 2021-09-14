---
title: Сообщение MM_MIM_CLOSE (Ммсистем. h)
description: сообщение о \_ \_ закрытии MIM MM отправляется в окно при закрытии входного устройства MIDI.
ms.assetid: 261021aa-4df6-44d8-aad3-5f98b1213459
keywords:
- сообщение MM_MIM_CLOSE Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_MIM_CLOSE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d8ce511365b1faa49faefaf4ed25c5b8befb2288
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127265939"
---
# <a name="mm_mim_close-message"></a>\_сообщение о \_ закрытии MIM MM

сообщение **о \_ \_ закрытии MIM MM** отправляется в окно при закрытии входного устройства MIDI.


```C++
MM_MIM_CLOSE 
wParam = (WPARAM) hInput 
lParam = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hInput"></span><span id="hinput"></span><span id="HINPUT"></span>*хинпут*
</dt> <dd>

Обработано устройство ввода MIDI, которое было закрыто.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Процессу не используйте.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

После отправки этого сообщения маркер устройства больше не действителен.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Цифровой интерфейс музыкальных инструментов (MIDI)](musical-instrument-digital-interface--midi.md)
</dt> <dt>

[Сообщения MIDI](midi-messages.md)
</dt> </dl>

 

 





