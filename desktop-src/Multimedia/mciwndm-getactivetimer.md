---
title: Сообщение MCIWNDM_GETACTIVETIMER (VFW. h)
description: Сообщение МЦИВНДМ \_ жетактиветимер получает период обновления, используемый, когда окно мЦивнд является активным окном. Это сообщение можно отправить явно или с помощью макроса МЦивнджетактиветимер.
ms.assetid: f9e6f9ed-75fd-4e45-ad92-79a82d8d572c
keywords:
- сообщение MCIWNDM_GETACTIVETIMER Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETACTIVETIMER
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4cb86fc2940c8bd5d82c004754b81e5389ada892
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470263"
---
# <a name="mciwndm_getactivetimer-message"></a>\_Сообщение мЦивндм жетактиветимер

Сообщение **мЦивндм \_ жетактиветимер** получает период обновления, используемый, когда окно мЦивнд является активным окном. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetactivetimer) .


```C++
MCIWNDM_GETACTIVETIMER 
wParam = 0; 
lParam = 0L; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает период обновления в миллисекундах. Значение по умолчанию — 500 миллисекунд.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивнджетактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetactivetimer)
</dt> </dl>

 

 





