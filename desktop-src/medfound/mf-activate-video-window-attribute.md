---
description: Обработчик для окна обрезки видео.
ms.assetid: 883bc7cf-f52f-4cb5-a942-b42b429b17a9
title: Атрибут MF_ACTIVATE_VIDEO_WINDOW (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5249d98f7a3850d68e83be43cb851c4089253ba7fc782724631a2983285c9ce0
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119826934"
---
# <a name="mf_activate_video_window-attribute"></a>\_Порт MF \_ активировать \_ атрибут окна видео

Обработчик для окна обрезки видео.

## <a name="data-type"></a>Тип данных

**UINT64**

Рассматривать как **DWORD \_ ptr** (**HWND**).

## <a name="remarks"></a>Remarks

Этот атрибут применяется к объекту активации расширенного обработчика видео (Евр). Значение задается автоматически при вызове [**мфкреатевидеорендерерактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatevideorendereractivate) для создания объекта активации Евр.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Расширенные атрибуты модуля подготовки видео](enhanced-video-renderer-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64)
</dt> <dt>

[**Имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64)
</dt> <dt>

[Объекты активации](activation-objects.md)
</dt> </dl>

 

 




