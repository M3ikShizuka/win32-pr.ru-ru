---
description: Позволяет расширенному обработчику видео (Евр) повысить производительность, используя для этого Bob-чересстрочную развертку.
ms.assetid: e145e862-b987-4962-a94b-f8370bbcd5ac
title: Атрибут EVRConfig_AllowDropToBob (UUIDs. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3940edd0945999f7300060d963806e3572a5d0fa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172212"
---
# <a name="evrconfig_allowdroptobob-attribute"></a>Еврконфиг \_ алловдроптобоб, атрибут

Позволяет расширенному обработчику видео (Евр) повысить производительность, используя для этого Bob-чересстрочную развертку.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="remarks"></a>Комментарии

Этот атрибут можно задать в приемнике Еврмедиа. Чтобы задать атрибут, **QueryInterface** будет запрашивать приемник мультимедиа Евр для интерфейса [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) .

Установка этого атрибута оказывает тот же результат, что и установка флага **мфвидеомикспрефс \_ АЛЛОВДРОПТОБОБ** в Евр. Описание этого флага см. в разделе [**мфвидеомикспрефс**](/windows/desktop/api/evr/ne-evr-mfvideomixprefs) .

Константа GUID для этого атрибута экспортируется из стрмиидс. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                            |
| Заголовок<br/>                   | <dl> <dt>UUID. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты Евр](enhanced-video-renderer-attributes.md)
</dt> <dt>

[Управление качеством видео](video-quality-management.md)
</dt> </dl>

 

 




