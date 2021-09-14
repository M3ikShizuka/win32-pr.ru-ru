---
description: Указывает пользовательские первичные цвета для типа видеоклипа.
ms.assetid: dc5df755-53cf-4910-af42-309f1f46b1ed
title: Атрибут MF_MT_CUSTOM_VIDEO_PRIMARIES (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3286d63e39638f74cacafa1b4376b28c7703f7c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127364052"
---
# <a name="mf_mt_custom_video_primaries-attribute"></a>\_ \_ \_ Атрибут пользовательского первичного элемента видео MF MT \_

Указывает пользовательские первичные цвета для типа видеоклипа.

## <a name="data-type"></a>Тип данных

**UINT32**

массив байтов;

## <a name="remarks"></a>Remarks

Данные атрибута являются [**пользовательской структурой \_ \_ \_ первичного цвета видео**](/windows/desktop/api/mfapi/ns-mfapi-mt_custom_video_primaries) .

Этот атрибут определяет фактический цветовой объем содержимого или изображения. CEA-861,3/SMPTE ST. 2086 сведения об основных томах хранятся в этом атрибуте декодерами. Обратите внимание на то, что этот атрибут не заменяет атрибут [**\_ \_ \_ первичного видео в MF MT**](mf-mt-video-primaries-attribute.md). Этот атрибут описывает подсказку о цветовой громкости содержимого, тогда как **\_ \_ \_ первичные цвета видео MF MT** описывают цветовые цвета, в которых содержимое фактически закодировано (например, значение 1,0 в каналах R/g/B представления с плавающей запятой).

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob)
</dt> <dt>

[**Имфаттрибутес:: SetBlob**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setblob)
</dt> <dt>

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)
</dt> </dl>

 

 




