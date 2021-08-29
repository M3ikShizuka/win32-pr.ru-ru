---
title: Сообщение MM_WIM_OPEN (Ммсистем. h)
description: '\_ \_ При открытии входного устройства с звуковой звукозаписью в окне будет отправлено сообщение с открытым WIM-файлом.'
ms.assetid: 4c646f58-c324-467e-871b-8fc36d5b89bc
keywords:
- сообщение MM_WIM_OPEN Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_WIM_OPEN
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4dc5271f4e2a49b762273b241133ea5c5826ebf1861ba9fe5eb4cf7832b164fe
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119065444"
---
# <a name="mm_wim_open-message"></a>MM \_ , \_ сообщение Open WIM

При открытии входного устройства с звуковой звукозаписью в окне будет отправлено сообщение с **\_ \_ открытым WIM** -файлом.


```C++
MM_WIM_OPEN 
wParam = (WPARAM) hInputDev 
lParam = reserved 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hInputDev"></span><span id="hinputdev"></span><span id="HINPUTDEV"></span>*хинпутдев*
</dt> <dd>

Обработчик для открытого устройства.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
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

 

 





