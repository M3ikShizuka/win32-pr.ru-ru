---
description: Указывает типы кадра синхронизации, которые поддерживаются потоком видео H. 264.
ms.assetid: A2E548F1-A5FA-4110-AD07-46BE9D7DC4A5
title: Атрибут MF_MT_H264_SUPPORTED_SYNC_FRAME_TYPES (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c328cbdef60750f2df7e9af403d8748c37d53b28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460936"
---
# <a name="mf_mt_h264_supported_sync_frame_types-attribute"></a>\_ \_ \_ \_ \_ Атрибут типов кадров синхронизации MF MT H264 Single bitrate поддерживается \_

Указывает типы кадра синхронизации, которые поддерживаются потоком видео H. 264.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="applies-to"></a>Применяется к

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)

## <a name="remarks"></a>Remarks

Этот атрибут применяется к типам носителей для потоков H. 264, переданных по USB. Значение соответствует полю **бмсуппортедсинкфраметипес** в дескрипторе формата видео УВК 1,5 H. 264.

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

 

 




