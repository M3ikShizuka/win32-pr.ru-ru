---
title: Сообщение WIM_CLOSE (Ммсистем. h)
description: Сообщение о \_ закрытии WIM отправляется в указанную функцию обратного вызова звукового сигнала аудио при закрытии устройства ввода аудио-сигнала. После отправки этого сообщения маркер устройства больше не действителен.
ms.assetid: 3774b8b4-b03b-49e7-b9cd-cf3f194df847
keywords:
- сообщение WIM_CLOSE Windows мультимедиа
topic_type:
- apiref
api_name:
- WIM_CLOSE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7488ef0d8a6a0d36852faa93397f853efb4f76f41761b6f38dd544ddcbc398ad
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119803894"
---
# <a name="wim_close-message"></a>\_Сообщение о закрытии WIM

Сообщение **о \_ закрытии WIM** отправляется в указанную функцию обратного вызова звукового сигнала аудио при закрытии устройства ввода аудио-сигнала. После отправки этого сообщения маркер устройства больше не действителен.


```C++
WIM_CLOSE 
dwParam1 = reserved 
dwParam2 = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="dwParam1"></span><span id="dwparam1"></span><span id="DWPARAM1"></span>*dwParam1*
</dt> <dd>

Процессу должно быть равно нулю.

</dd> <dt>

<span id="dwParam2"></span><span id="dwparam2"></span><span id="DWPARAM2"></span>*dwParam2*
</dt> <dd>

Процессу должно быть равно нулю.

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

[Звуковая волна](waveform-audio.md)
</dt> <dt>

[Сообщения волны](waveform-messages.md)
</dt> </dl>

 

 





