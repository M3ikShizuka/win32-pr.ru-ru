---
title: Сообщение MCIWNDM_GETSPEED (VFW. h)
description: Сообщение МЦИВНДМ \_ Speed получает скорость воспроизведения устройства MCI. Это сообщение можно отправить явно или с помощью макроса МЦивнджетспид.
ms.assetid: d10a8f88-e85e-449b-8655-bb0832031d59
keywords:
- сообщение MCIWNDM_GETSPEED Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETSPEED
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c84a8ebb3e97d4543f68f3a237add8eed7706ae2
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370674"
---
# <a name="mciwndm_getspeed-message"></a>\_Сообщение МЦИВНДМ Speed

Сообщение **МЦИВНДМ \_ Speed** получает скорость воспроизведения устройства MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетспид**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetspeed) .


```C++
MCIWNDM_GETSPEED 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

При успешном выполнении возвращает скорость воспроизведения. Значение обычной скорости — 1000. Большие значения указывают более быстрые скорости, а меньшие значения — медленные.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивнджетспид**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetspeed)
</dt> </dl>

 

 





