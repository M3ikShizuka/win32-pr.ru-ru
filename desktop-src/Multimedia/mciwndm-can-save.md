---
title: Сообщение MCIWNDM_CAN_SAVE (VFW. h)
description: МЦИВНДМ \_ может \_ сохранить сообщение, определяет, может ли устройство MCI сохранять данные. Это сообщение можно отправить явно или с помощью макроса МЦивндкансаве.
ms.assetid: b4e27190-b095-494b-9ed3-10653bea187b
keywords:
- сообщение MCIWNDM_CAN_SAVE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_CAN_SAVE
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 11b60b8a5d93ac80befc8beeb6665399efe44f1e
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370620"
---
# <a name="mciwndm_can_save-message"></a>МЦИВНДМ \_ может \_ сохранить сообщение

**МЦивндм \_ может \_ сохранить** сообщение, определяет, может ли устройство MCI сохранять данные. Это сообщение можно отправить явно или с помощью макроса [**мЦивндкансаве**](/windows/desktop/api/Vfw/nf-vfw-mciwndcansave) .


```C++
MCIWNDM_CAN_SAVE 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если устройство поддерживает сохранение или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндкансаве**](/windows/desktop/api/Vfw/nf-vfw-mciwndcansave)
</dt> </dl>

 

 





