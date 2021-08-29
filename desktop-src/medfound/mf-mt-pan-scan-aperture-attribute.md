---
description: Определяет апертуру и сканирование, т. е. 4&\# 215; 3 региона видео, который должен отображаться в режиме панорамирования и сканирования.
ms.assetid: faa577fd-6572-46b9-9c6c-f91c47832cb5
title: Атрибут MF_MT_PAN_SCAN_APERTURE (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 61d9b8d4ed5e8fe8887c229d83ffc276bf4d90b968834161ab60cc5d102095bb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119940614"
---
# <a name="mf_mt_pan_scan_aperture-attribute"></a>\_ \_ \_ Атрибут апертуры развертки MF MT \_

Определяет апертуру и сканирование, то есть 4 × 3 региона видео, который должен отображаться в режиме панорамы и сканирования.

## <a name="data-type"></a>Тип данных

массив байтов;

## <a name="remarks"></a>Remarks

Значение атрибута является структурой [**мфвидеоареа**](/windows/desktop/api/mfobjects/ns-mfobjects-mfvideoarea) .

Этот атрибут используется для обрезки широкоэкранных видео до 4:3 пропорций. Апертура/развертка используется только в режиме панорамирования/развертки, который включается путем установки атрибута « [**\_ \_ \_ \_ Включить сканирование MF MT Pan**](mf-mt-pan-scan-enabled-attribute.md) » в **значение true**.

Если режим Pan/Scan не включен, используйте апертуру экрана, заданную атрибутом [**\_ \_ \_ \_ апертуры по крайней мере в MF MT**](mf-mt-minimum-display-aperture-attribute.md) .

Если этот атрибут не задан, то раскадровка панорамы и развертки считается кадром всего видео.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Приложения UWP для классических приложений Vista \|\]<br/>                              |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для классических приложений сервера 2008 \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Мфапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> <dt>

[Пропорции рисунка](picture-aspect-ratio.md)
</dt> <dt>

[Типы видеоклипов](video-media-types.md)
</dt> <dt>

[**Имфаттрибутес:: BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob)
</dt> <dt>

[**Имфаттрибутес:: SetBlob**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setblob)
</dt> <dt>

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)
</dt> <dt>

[**\_ \_ геометрическое \_ Апертура MF**](mf-mt-geometric-aperture-attribute.md)
</dt> <dt>

[**\_ \_ Минимальный \_ \_ Апертура экрана MF MT**](mf-mt-minimum-display-aperture-attribute.md)
</dt> <dt>

[**\_ \_ включена проверка панорамы MF MT \_ \_**](mf-mt-pan-scan-enabled-attribute.md)
</dt> </dl>

 

 




