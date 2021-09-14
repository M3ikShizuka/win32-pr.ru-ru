---
title: Сообщение MM_MIM_ERROR (Ммсистем. h)
description: '\_ \_ сообщение об ошибке MM MIM отправляется в окно при получении недопустимого сообщения MIDI.'
ms.assetid: 03760bfc-a4ef-48cd-97a9-1b93b56fc641
keywords:
- сообщение MM_MIM_ERROR Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_MIM_ERROR
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 76b45988259601b40a804f9eb8acfbb085bddcda
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127265936"
---
# <a name="mm_mim_error-message"></a>MM \_ MIM \_ сообщение об ошибке

сообщение **\_ \_ об ошибке MM MIM** отправляется в окно при получении недопустимого сообщения MIDI.


```C++
MM_MIM_ERROR 
wParam = (WPARAM) hInput 
lParam = (LPARAM) (DWORD) lMidiMessage 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hInput"></span><span id="hinput"></span><span id="HINPUT"></span>*хинпут*
</dt> <dd>

Обрабатывает входное устройство MIDI, которое получило недопустимое сообщение.

</dd> <dt>

<span id="lMidiMessage"></span><span id="lmidimessage"></span><span id="LMIDIMESSAGE"></span>*лмидимессаже*
</dt> <dd>

Недопустимое сообщение MIDI. Сообщение упаковывается в значение **DWORD** с первым байтом сообщения в байте нижнего порядка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

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

 

 





