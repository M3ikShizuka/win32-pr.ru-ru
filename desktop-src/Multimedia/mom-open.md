---
title: Сообщение MOM_OPEN (Ммсистем. h)
description: Сообщение о \_ открытом вызове MOM отправляется в функцию обратного вызова MIDI OUTPUT при открытии выходного устройства MIDI.
ms.assetid: f3360482-7d16-419c-b5d1-0dd3a6e3c690
keywords:
- сообщение MOM_OPEN Windows мультимедиа
topic_type:
- apiref
api_name:
- MOM_OPEN
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 650291df51382640da2c3b4fb21910da4271ca96ace2d5711558d43501080795
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120038844"
---
# <a name="mom_open-message"></a>\_Открытое сообщение MOM

Сообщение **о \_ открытом** вызове MOM отправляется в функцию обратного вызова MIDI OUTPUT при открытии выходного устройства MIDI.


```C++
MOM_OPEN 
dwParam1 = reserved 
dwParam2 = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="dwParam1"></span><span id="dwparam1"></span><span id="DWPARAM1"></span>*dwParam1*
</dt> <dd>

Процессу не используйте.

</dd> <dt>

<span id="dwParam2"></span><span id="dwparam2"></span><span id="DWPARAM2"></span>*dwParam2*
</dt> <dd>

Процессу не используйте.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Сообщения MIDI](midi-messages.md)
</dt> </dl>

 

 





