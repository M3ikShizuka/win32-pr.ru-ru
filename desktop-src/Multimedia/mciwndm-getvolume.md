---
title: Сообщение MCIWNDM_GETVOLUME (VFW. h)
description: Сообщение МЦИВНДМ \_ . Volume получает текущую настройку тома для устройства MCI. Это сообщение можно отправить явно или с помощью макроса МЦивнджетволуме.
ms.assetid: 3f1de023-4da8-4899-accc-409701d6e921
keywords:
- сообщение MCIWNDM_GETVOLUME Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETVOLUME
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4aa11fb13a56dda7cb83e3d6c98b4b66083e91b9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057455"
---
# <a name="mciwndm_getvolume-message"></a>\_Сообщение мЦивндм

Сообщение **мЦивндм. \_ Volume** получает текущую настройку тома для устройства MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетволуме**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetvolume) .


```C++
MCIWNDM_GETVOLUME 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает текущий параметр тома. Значение по умолчанию ― 1000. Более высокие значения указывают громкости, а низкие значения указывают на незвуковые тома.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**мЦивнджетволуме**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetvolume)
</dt> </dl>

 

 





