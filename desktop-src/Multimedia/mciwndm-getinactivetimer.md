---
title: Сообщение MCIWNDM_GETINACTIVETIMER (VFW. h)
description: Сообщение МЦИВНДМ \_ жетинактиветимер получает период обновления, используемый, когда окно мЦивнд является неактивным окном. Это сообщение можно отправить явно или с помощью макроса МЦивнджетинактиветимер.
ms.assetid: 84e00d2f-2cf8-4b6b-a8cb-7eb320754783
keywords:
- сообщение MCIWNDM_GETINACTIVETIMER Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETINACTIVETIMER
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0ec8de85796139b98e76d631a9386493752dad9942241069a7f1a5ab535fab72
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120038084"
---
# <a name="mciwndm_getinactivetimer-message"></a>\_Сообщение мЦивндм жетинактиветимер

Сообщение **мЦивндм \_ жетинактиветимер** получает период обновления, используемый, когда окно мЦивнд является неактивным окном. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетинактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetinactivetimer) .


```C++
MCIWNDM_GETINACTIVETIMER 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает период обновления в миллисекундах. Значение по умолчанию — 2000 миллисекунд.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивнджетинактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetinactivetimer)
</dt> </dl>

 

 





