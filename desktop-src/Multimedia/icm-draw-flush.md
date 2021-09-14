---
title: Сообщение ICM_DRAW_FLUSH (VFW. h)
description: '\_ \_ Сообщение о сбросе ICM Draw уведомляет драйвер подготовки, чтобы отобразить содержимое всех буферов изображений, которые ожидают прорисовки. Это сообщение можно отправить явно или с помощью макроса Икдравфлуш.'
ms.assetid: c29ed751-c773-4476-98fe-6edef3ff0cf4
keywords:
- сообщение ICM_DRAW_FLUSH Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_FLUSH
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 38ec42c51222313f7d3599c3b4f264dbd21a9434
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147478"
---
# <a name="icm_draw_flush-message"></a>\_Сообщение о \_ сбросе ICM Draw

Сообщение **о \_ \_ сбросе ICM Draw** уведомляет драйвер подготовки, чтобы отобразить содержимое всех буферов изображений, которые ожидают прорисовки. Это сообщение можно отправить явно или с помощью макроса [**икдравфлуш**](/windows/desktop/api/Vfw/nf-vfw-icdrawflush) .


```C++
ICM_DRAW_FLUSH 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Это сообщение используется только оборудованием, которое выполняет собственное асинхронное распаковка, время и рисование.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Диспетчер сжатия видео](video-compression-manager.md)
</dt> <dt>

[Сообщения о сжатии видео](video-compression-messages.md)
</dt> </dl>

 

 





