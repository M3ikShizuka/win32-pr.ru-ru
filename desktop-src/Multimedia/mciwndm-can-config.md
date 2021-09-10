---
title: Сообщение MCIWNDM_CAN_CONFIG (VFW. h)
description: Сообщение МЦИВНДМ \_ Can \_ config определяет, может ли устройство MCI отобразить диалоговое окно конфигурации. Это сообщение можно отправить явно или с помощью макроса МЦивндканконфиг.
ms.assetid: f1eb22a8-d0fc-4d2c-a414-392e560cfbed
keywords:
- сообщение MCIWNDM_CAN_CONFIG Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_CAN_CONFIG
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 816a8c1dfaec6fc7d7854f8873ce05e74e4de6bc
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370608"
---
# <a name="mciwndm_can_config-message"></a>МЦИВНДМ \_ может \_ сообщение конфигурации

Сообщение **мЦивндм \_ Can \_ config** определяет, может ли устройство MCI отобразить диалоговое окно конфигурации. Это сообщение можно отправить явно или с помощью макроса [**мЦивндканконфиг**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanconfig) .


```C++
MCIWNDM_CAN_CONFIG 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если устройство поддерживает конфигурацию, или **значение false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндканконфиг**](/windows/desktop/api/Vfw/nf-vfw-mciwndcanconfig)
</dt> </dl>

 

 





