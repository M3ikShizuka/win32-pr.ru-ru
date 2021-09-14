---
description: Указывает количество конечных точек потоковой передачи и число поддерживаемых потоков для кодировщика УВК H. 264.
ms.assetid: 343EC59E-30E5-4F37-8B05-60EF51717835
title: Атрибут MF_MT_H264_SIMULCAST_SUPPORT (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 879490c6984186cf45971d2b122f0c2217b0f164
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460940"
---
# <a name="mf_mt_h264_simulcast_support-attribute"></a>\_Атрибут поддержки MF MT \_ H264 Single bitrate \_ транслироваться \_

Указывает количество конечных точек потоковой передачи и число поддерживаемых потоков для кодировщика УВК H. 264.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="applies-to"></a>Применяется к

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)

## <a name="remarks"></a>Remarks

Этот атрибут применяется к типам носителей для потоков H. 264, переданных по USB. Значение соответствует полю **бсимулкастсуппорт** в дескрипторе формата видео УВК 1,5 H. 264.

Этот атрибут также используется с [кодировщиками камер H. 264 увк 1,5](camera-encoder-h264-uvc-1-5.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ приложения UWP для классических приложений \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Мфапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> </dl>

 

 




