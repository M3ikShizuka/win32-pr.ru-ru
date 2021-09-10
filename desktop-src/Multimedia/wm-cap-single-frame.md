---
title: Сообщение WM_CAP_SINGLE_FRAME (VFW. h)
description: Сообщение с \_ \_ одним \_ кадром WM Cap добавляет один кадр в файл записи, Открытый с помощью \_ \_ \_ сообщения об открытом фрейме WM Cap \_ . Это сообщение можно отправить явно или с помощью макроса Капкаптуресинглефраме.
ms.assetid: 95466961-0719-4ff7-afc8-f7bf0e0974ac
keywords:
- сообщение WM_CAP_SINGLE_FRAME Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_SINGLE_FRAME
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a919036ee38fdcf00f55c3d4044cd3f45bd13c82
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371532"
---
# <a name="wm_cap_single_frame-message"></a>\_ \_ \_ Сообщение об одном кадре WM Cap

Сообщение **с \_ \_ одним \_ кадром WM Cap** добавляет один кадр в файл записи, Открытый с помощью сообщения об [**\_ \_ \_ \_ открытом фрейме WM Cap**](wm-cap-single-frame-open.md) . Это сообщение можно отправить явно или с помощью макроса [**капкаптуресинглефраме**](/windows/desktop/api/Vfw/nf-vfw-capcapturesingleframe) .


```C++
WM_CAP_SINGLE_FRAME 
wParam = (WPARAM) 0; 
lParam = 0L; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

 





