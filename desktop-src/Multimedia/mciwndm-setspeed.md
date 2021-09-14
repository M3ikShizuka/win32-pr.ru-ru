---
title: Сообщение MCIWNDM_SETSPEED (VFW. h)
description: Сообщение МЦИВНДМ \_ сетспид задает скорость воспроизведения устройства MCI. Это сообщение можно отправить явно или с помощью макроса МЦивндсетспид.
ms.assetid: 7658dd25-dc68-4bd1-b995-df06b509be16
keywords:
- сообщение MCIWNDM_SETSPEED Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_SETSPEED
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 282bb3a2e135b674605be55aaccaa455d30edbcc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250738"
---
# <a name="mciwndm_setspeed-message"></a>\_Сообщение мЦивндм сетспид

Сообщение **мЦивндм \_ сетспид** задает скорость воспроизведения устройства MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивндсетспид**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetspeed) .


```C++
MCIWNDM_SETSPEED 
wParam = 0; 
lParam = (LPARAM) (UINT) iSpeed; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="iSpeed"></span><span id="ispeed"></span><span id="ISPEED"></span>*испид*
</dt> <dd>

Скорость воспроизведения. Укажите 1000 для обычной скорости, более высокие значения для более быстрых скоростей и меньшие значения для медленных скоростей.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивндсетспид**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetspeed)
</dt> </dl>

 

 





