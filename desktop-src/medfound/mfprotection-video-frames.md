---
description: Указывает, разрешено ли приложению доступ к несжатым видеокадрам.
ms.assetid: 7D2A9003-B36E-4082-877E-8AC7F5645E89
title: Атрибут MFPROTECTION_VIDEO_FRAMES (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 67a8ccfc56fb1c1b52b14e16d8e702111f3d8564
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462026"
---
# <a name="mfprotection_video_frames-attribute"></a>\_Атрибут "кадры видео мфпротектион" \_

Указывает, разрешено ли приложению доступ к несжатым видеокадрам.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Значение 0 указывает, что приложению разрешен доступ к кадрам. Это может быть определено в результате применения частного соглашения между приложением и определенной системой защиты содержимого.

Значение 1 указывает, что приложению разрешен доступ к кадрам, если приложение предоставляет действительный сертификат приложения (см. раздел [**имфмедиаенгинепротектедконтент:: сетаппликатионцертификате**](/windows/desktop/api/mfmediaengine/nf-mfmediaengine-imfmediaengineprotectedcontent-setapplicationcertificate)).

Значение 0xFFFFFFFF, которое является значением по умолчанию, указывает, что приложениям не разрешен доступ к несжатым кадрам.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ Только приложения UWP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ Только приложения UWP\]<br/>                                   |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> </dl>

 

 




