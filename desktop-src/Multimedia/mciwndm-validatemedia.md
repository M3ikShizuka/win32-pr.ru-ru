---
title: Сообщение MCIWNDM_VALIDATEMEDIA (VFW. h)
description: Сообщение МЦИВНДМ \_ валидатемедиа обновляет начальные и конечные расположения содержимого, текущую положение в содержимом и значение TrackBar в соответствии с текущим форматом времени.
ms.assetid: 98ac6227-fc90-4276-8e26-2bd005e35dc6
keywords:
- сообщение MCIWNDM_VALIDATEMEDIA Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_VALIDATEMEDIA
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2db79f5714a9f48a2fdd73ff6eedecd0a14172e352e0a40ffbdccdd3aaaf4c2f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119428534"
---
# <a name="mciwndm_validatemedia-message"></a>\_Сообщение мЦивндм валидатемедиа

Сообщение **мЦивндм \_ валидатемедиа** обновляет начальные и конечные расположения содержимого, текущую положение в содержимом и значение TrackBar в соответствии с текущим форматом времени. Это сообщение можно отправить явно или с помощью макроса [**мЦивндвалидатемедиа**](/windows/desktop/api/Vfw/nf-vfw-mciwndvalidatemedia) .


```C++
MCIWNDM_VALIDATEMEDIA 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Как правило, использовать этот макрос не требуется. Однако, если приложение изменяет формат времени устройства без использования МЦивнд; начальное и конечное расположение содержимого, а также значение TrackBar, продолжайте использовать старый формат. Этот макрос можно использовать для обновления этих значений.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивндвалидатемедиа**](/windows/desktop/api/Vfw/nf-vfw-mciwndvalidatemedia)
</dt> </dl>

 

 





