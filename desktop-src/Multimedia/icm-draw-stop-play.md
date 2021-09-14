---
title: Сообщение ICM_DRAW_STOP_PLAY (VFW. h)
description: '\_ \_ \_ При завершении операции воспроизведения выводится сообщение о том, что средство ICM Draw останавливает воспроизведение уведомляет драйвер подготовки. Это сообщение можно отправить явно или с помощью макроса Икдравстопплай.'
ms.assetid: cfe2ee98-80d0-4554-bcbd-9873769da674
keywords:
- сообщение ICM_DRAW_STOP_PLAY Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_STOP_PLAY
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea3964b623c93d452ab7bf9a32c6b9d9b1573fec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246319"
---
# <a name="icm_draw_stop_play-message"></a>\_Сообщение о \_ зависании при прорисовке \_

При завершении операции воспроизведения выводится сообщение о том, что средство **ICM \_ Draw \_ останавливает \_ Воспроизведение** уведомляет драйвер подготовки. Это сообщение можно отправить явно или с помощью макроса [**икдравстопплай**](/windows/desktop/api/Vfw/nf-vfw-icdrawstopplay) .


```C++
ICM_DRAW_STOP_PLAY 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Это сообщение используется по завершении операции воспроизведения. Используйте сообщение об ошибке [**ICM \_ Draw \_**](icm-draw-stop.md) для окончания времени.

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

 

 





