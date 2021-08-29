---
description: Заставляет Расширенный модуль подготовки видео (Евр) пропускать второе поле каждого кадра с чередованием.
ms.assetid: b79d9230-b127-4e9b-b73b-685ce27aefa9
title: Атрибут EVRConfig_ForceHalfInterlace (UUIDs. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cf3d73eceb1728b8bdc043ba69ee62249783ee109c29ff173a9e563f68505d9b
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120061594"
---
# <a name="evrconfig_forcehalfinterlace-attribute"></a>Еврконфиг \_ форцехалфинтерлаце, атрибут

Заставляет Расширенный модуль подготовки видео (Евр) пропускать второе поле каждого кадра с чередованием.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="remarks"></a>Remarks

Этот атрибут можно задать в приемнике носителей Евр. Чтобы задать атрибут, используйте **QueryInterface** , чтобы запросить приемник мультимедиа Евр для интерфейса [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) .

Установка этого атрибута оказывает тот же результат, что и установка флага **мфвидеомикспрефс \_ ФОРЦЕХАЛФИНТЕРЛАЦЕ** в Евр. Описание этого флага см. в разделе [**мфвидеомикспрефс**](/windows/desktop/api/evr/ne-evr-mfvideomixprefs) .

Константа GUID для этого атрибута экспортируется из стрмиидс. lib.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                            |
| Заголовок<br/>                   | <dl> <dt>UUID. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты Евр](enhanced-video-renderer-attributes.md)
</dt> <dt>

[Управление качеством видео](video-quality-management.md)
</dt> </dl>

 

 




