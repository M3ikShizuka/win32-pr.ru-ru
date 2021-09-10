---
title: Сообщение MCIWNDM_EJECT (VFW. h)
description: Сообщение о \_ извлечении мЦивндм отправляет команду на устройство MCI для извлечения носителя. Это сообщение можно отправить явно или с помощью макроса МЦивндежект.
ms.assetid: a492f504-8b58-480e-9766-bc2878466c44
keywords:
- сообщение MCIWNDM_EJECT Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_EJECT
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e41686ce41b82dc48ee6c22ac556606c79c5b24a
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370626"
---
# <a name="mciwndm_eject-message"></a>\_Сообщение о извлечении мЦивндм

Сообщение **о \_ извлечении мЦивндм** отправляет команду на устройство MCI для извлечения носителя. Это сообщение можно отправить явно или с помощью макроса [**мЦивндежект**](/windows/desktop/api/Vfw/nf-vfw-mciwndeject) .


```C++
MCIWNDM_EJECT 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндежект**](/windows/desktop/api/Vfw/nf-vfw-mciwndeject)
</dt> </dl>

 

 





