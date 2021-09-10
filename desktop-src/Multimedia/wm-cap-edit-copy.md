---
title: Сообщение WM_CAP_EDIT_COPY (VFW. h)
description: '\_ \_ Сообщение об изменении копии с креплениями WM \_ копирует содержимое буфера кадров видео и связанной с ним палитры в буфер обмена. Это сообщение можно отправить явно или с помощью макроса Капедиткопи.'
ms.assetid: 16f1dd7d-af4d-4096-add8-eec5f0a0607f
keywords:
- сообщение WM_CAP_EDIT_COPY Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_EDIT_COPY
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bb81c21fc10846adaa113c02b6250bbb35cfff50
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371421"
---
# <a name="wm_cap_edit_copy-message"></a>\_ \_ Сообщение об изменении копии с КРЕПЛЕНИЯми WM \_

Сообщение **об \_ \_ изменении \_ копии с креплениями WM** копирует содержимое буфера кадров видео и связанной с ним палитры в буфер обмена. Это сообщение можно отправить явно или с помощью макроса [**капедиткопи**](/windows/desktop/api/Vfw/nf-vfw-capeditcopy) .


```C++
WM_CAP_EDIT_COPY 
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

 

 





