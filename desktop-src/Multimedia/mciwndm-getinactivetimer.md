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
ms.openlocfilehash: a270aeffdee59b7749aa87a0e711204960d74d7f
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370653"
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



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивнджетинактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetinactivetimer)
</dt> </dl>

 

 





