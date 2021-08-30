---
title: Сообщение MCIWNDM_SETOWNER (VFW. h)
description: Сообщение МЦИВНДМ \_ сетовнер указывает, что окно будет принимать сообщения уведомления, связанные с окном мЦивнд. Это сообщение можно отправить явно или с помощью макроса МЦивндсетовнер.
ms.assetid: c2d0f9d5-bf60-4036-a613-65ba1ed83110
keywords:
- сообщение MCIWNDM_SETOWNER Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_SETOWNER
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2a45fb1f7893641fe1e1f4f0bb2e79b31f33c465811e9dec83869af90d819414
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119807754"
---
# <a name="mciwndm_setowner-message"></a>\_Сообщение мЦивндм сетовнер

Сообщение **мЦивндм \_ сетовнер** указывает, что окно будет принимать сообщения уведомления, связанные с окном мЦивнд. Это сообщение можно отправить явно или с помощью макроса [**мЦивндсетовнер**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetowner) .


```C++
MCIWNDM_SETOWNER 
wParam = (WPARAM) hwndP; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hwndP"></span><span id="hwndp"></span><span id="HWNDP"></span>*хвндп*
</dt> <dd>

Обработчик для окна, получающего сообщения уведомления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ноль.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндсетовнер**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetowner)
</dt> </dl>

 

 





