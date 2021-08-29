---
title: Сообщение MCIWNDM_CAN_WINDOW (VFW. h)
description: МЦИВНДМ \_ может \_ поwindow Message определяет, поддерживает ли устройство MCI команды MCI, ориентированные на окна. Это сообщение можно отправить явно или с помощью макроса МЦивндканвиндов.
ms.assetid: bf89c096-1272-441e-9334-2b4215dbc979
keywords:
- сообщение MCIWNDM_CAN_WINDOW Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_CAN_WINDOW
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 26db92a07437f10295c2670e035950be5a56813aa6bb4c6252cfe35ef502f77c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120038154"
---
# <a name="mciwndm_can_window-message"></a>МЦИВНДМ \_ может \_ пооконное сообщение

**МЦивндм \_ может \_ поwindow** Message определяет, поддерживает ли устройство MCI команды MCI, ориентированные на окна. Это сообщение можно отправить явно или с помощью макроса [**мЦивндканвиндов**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanwindow) .


```C++
MCIWNDM_CAN_WINDOW 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если устройство поддерживает команды MCI, ориентированные на окна, или **false** в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндканвиндов**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanwindow)
</dt> </dl>

 

 





