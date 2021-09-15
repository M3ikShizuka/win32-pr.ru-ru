---
title: Сообщение MCIWNDM_CAN_RECORD (VFW. h)
description: МЦИВНДМ \_ может \_ записывать сообщение, определяет, поддерживает ли устройство MCI запись. Это сообщение можно отправить явно или с помощью макроса МЦивндканрекорд.
ms.assetid: b5a789fa-6a88-487d-a374-8f4798ee5a62
keywords:
- сообщение MCIWNDM_CAN_RECORD Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_CAN_RECORD
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2acbc9efa3ca973c12112a599d1202ad936107a9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470278"
---
# <a name="mciwndm_can_record-message"></a>МЦИВНДМ \_ может \_ записать сообщение

**МЦивндм \_ может \_ записывать** сообщение, определяет, поддерживает ли устройство MCI запись. Это сообщение можно отправить явно или с помощью макроса [**мЦивндканрекорд**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanrecord) .


```C++
MCIWNDM_CAN_RECORD 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если устройство поддерживает запись или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивндканрекорд**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanrecord)
</dt> </dl>

 

 





