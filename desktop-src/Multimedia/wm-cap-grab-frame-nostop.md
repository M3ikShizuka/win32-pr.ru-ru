---
title: Сообщение WM_CAP_GRAB_FRAME_NOSTOP (VFW. h)
description: Сообщение о \_ \_ \_ неостановкой кадра захвата для WM \_ замещает буфер кадров одним несжатым кадром с устройства записи и отображает его.
ms.assetid: 5f6e3ce7-3595-456e-82c8-eeb162ace81a
keywords:
- сообщение WM_CAP_GRAB_FRAME_NOSTOP Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_GRAB_FRAME_NOSTOP
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5073cf5eae44f564d24cd1ebb67193d8738fd77b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169491"
---
# <a name="wm_cap_grab_frame_nostop-message"></a>\_Сообщение о \_ \_ \_ неостановкой кадра захвата WM Cap

Сообщение **о \_ \_ \_ \_ Неостановкой кадра захвата для WM** замещает буфер кадров одним несжатым кадром с устройства записи и отображает его. В отличие от сообщения [**с \_ закреплением \_ \_ WM**](wm-cap-grab-frame.md) , состояние наложения или предварительного просмотра не изменяется этим сообщением. Это сообщение можно отправить явно или с помощью макроса [**капграбфраменостоп**](/windows/desktop/api/Vfw/nf-vfw-capgrabframenostop) .


```C++
WM_CAP_GRAB_FRAME_NOSTOP 
wParam = (WPARAM) 0; 
lParam = 0L; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** в противном случае.

## <a name="remarks"></a>Remarks

Дополнительные сведения об установке функций обратного вызова см. в разделе [**\_ \_ \_ \_ ошибка обратного вызова Set крепления WM**](wm-cap-set-callback-error.md) , а также сообщения [**\_ \_ \_ \_ кадра обратного вызова Set крепления WM**](wm-cap-set-callback-frame.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

 





