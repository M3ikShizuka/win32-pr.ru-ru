---
title: Сообщение WOM_DONE (Ммсистем. h)
description: Сообщение вом \_ done отправляется в функцию выходного обратного вызова звуковой волны, когда заданный выходной буфер возвращается приложению.
ms.assetid: cac94a44-d1b0-43de-b3ec-ae34547b1fc3
keywords:
- сообщение WOM_DONE Windows мультимедиа
topic_type:
- apiref
api_name:
- WOM_DONE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ab64598a2dfdd329615ca116fb6382909bb83b01
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245620"
---
# <a name="wom_done-message"></a>\_Сообщение о завершении ВОМ

Сообщение **вом \_ done** отправляется в функцию выходного обратного вызова звуковой волны, когда заданный выходной буфер возвращается приложению. Буферы возвращаются в приложение, когда они воспроизводятся, или в результате вызова функции [**вавеаутресет**](/windows/win32/api/mmeapi/nf-mmeapi-waveoutreset) .


```C++
WOM_DONE 
dwParam1 = (DWORD) lpwvhdr 
dwParam2 = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="dwParam1"></span><span id="dwparam1"></span><span id="DWPARAM1"></span>*dwParam1*
</dt> <dd>

Указатель на структуру [**вавехдр**](/windows/win32/api/mmeapi/ns-mmeapi-wavehdr) , определяющую буфер.

</dd> <dt>

<span id="dwParam2"></span><span id="dwparam2"></span><span id="DWPARAM2"></span>*dwParam2*
</dt> <dd>

Процессу должно быть равно нулю.

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

[Звуковая волна](waveform-audio.md)
</dt> <dt>

[Сообщения волны](waveform-messages.md)
</dt> </dl>

 

