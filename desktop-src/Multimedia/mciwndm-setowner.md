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
ms.openlocfilehash: c3989632e83a65cda5e805bd91da3f502ca387d6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250759"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивндсетовнер**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetowner)
</dt> </dl>

 

 





