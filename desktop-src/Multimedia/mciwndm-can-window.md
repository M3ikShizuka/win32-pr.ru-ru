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
ms.openlocfilehash: d638b61093483b6e834b57af1d5c892d77d0f1d4
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370611"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндканвиндов**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanwindow)
</dt> </dl>

 

 





