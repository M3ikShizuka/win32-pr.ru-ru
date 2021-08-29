---
title: Сообщение ICM_DRAW_RENDERBUFFER (VFW. h)
description: Сообщение ICM \_ Draw \_ рендербуффер уведомляет драйвер подготовки, чтобы вывести переданные ему кадры. Это сообщение можно отправить явно или с помощью макроса Икдраврендербуффер.
ms.assetid: b21be12c-b8a5-49ea-b6b3-d2eb0077a8e9
keywords:
- сообщение ICM_DRAW_RENDERBUFFER Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_RENDERBUFFER
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 28a5066d5aa129ffad98aa82eb8d09ba91c0e42fca4edae501f8a7c1775d4be8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119526134"
---
# <a name="icm_draw_renderbuffer-message"></a>\_Сообщение ICM Draw \_ рендербуффер

Сообщение **ICM \_ Draw \_ рендербуффер** уведомляет драйвер подготовки, чтобы вывести переданные ему кадры. Это сообщение можно отправить явно или с помощью макроса [**икдраврендербуффер**](/windows/desktop/api/Vfw/nf-vfw-icdrawrenderbuffer) .


```C++
ICM_DRAW_RENDERBUFFER 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Используйте это сообщение с оборудованием, которое выполняет собственное асинхронное распаковка, время и рисование.

Это сообщение обычно используется для выполнения операции поиска, когда драйверу необходимо специально указать отображение каждого кадра видео, переданного в него, а не воспроизведение последовательности видеокадров.

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

 

 





