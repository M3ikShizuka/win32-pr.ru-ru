---
title: Сообщение WIM_DATA (Ммсистем. h)
description: Сообщение с \_ данными WIM отправляется в указанную функцию обратного вызова аудио-звука, когда в входном буфере содержатся данные звуковой волны, а буфер возвращается приложению.
ms.assetid: 94cc02b8-61c4-44b9-9f8e-041fe989c1a6
keywords:
- сообщение WIM_DATA Windows мультимедиа
topic_type:
- apiref
api_name:
- WIM_DATA
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 28bcfdd249dda5621d4914d75d3ffc7b13e4d767
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371250"
---
# <a name="wim_data-message"></a>\_Сообщение данных WIM

Сообщение **с \_ данными WIM** отправляется в указанную функцию обратного вызова аудио-звука, когда в входном буфере содержатся данные звуковой волны, а буфер возвращается приложению. Сообщение может быть отправлено, когда буфер полон или после вызова функции [**вавеинресет**](/windows/win32/api/mmeapi/nf-mmeapi-waveinreset) .


```C++
WIM_DATA 
dwParam1 = (DWORD) lpwvhdr 
dwParam2 = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="dwParam1"></span><span id="dwparam1"></span><span id="DWPARAM1"></span>*dwParam1*
</dt> <dd>

Указатель на структуру [**вавехдр**](/windows/win32/api/mmeapi/ns-mmeapi-wavehdr) , определяющую буфер, содержащий данные.

</dd> <dt>

<span id="dwParam2"></span><span id="dwparam2"></span><span id="DWPARAM2"></span>*dwParam2*
</dt> <dd>

Процессу должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Возвращенный буфер может быть незаполненным. Используйте элемент **двбитесрекордед** структуры [**вавехдр**](/windows/win32/api/mmeapi/ns-mmeapi-wavehdr) , заданную параметром *лпввхдр* , чтобы определить число байтов, записанных в возвращенный буфер.

## <a name="requirements"></a>Требования



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

 

