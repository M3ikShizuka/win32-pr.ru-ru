---
title: Сообщение MCIWNDM_GETDEVICEID (VFW. h)
description: Сообщение МЦИВНДМ \_ GETDEVICEID получает идентификатор открытого устройства MCI для использования с функцией мЦисендкомманд. Это сообщение можно отправить явно или с помощью макроса МЦивнджетдевицеид.
ms.assetid: 188f15fa-579a-438e-a812-9a2b684127c0
keywords:
- сообщение MCIWNDM_GETDEVICEID Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETDEVICEID
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b2f2271b18dcf8f295594031ab2c7c80dd8dec06
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370641"
---
# <a name="mciwndm_getdeviceid-message"></a>\_Сообщение мЦивндм GETDEVICEID

Сообщение **мЦивндм \_ GETDEVICEID** получает идентификатор открытого устройства MCI для использования с функцией [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) . Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетдевицеид**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetdeviceid) .


```C++
MCIWNDM_GETDEVICEID 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает идентификатор устройства.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> <dt>

[**мЦивнджетдевицеид**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetdeviceid)
</dt> </dl>

 

