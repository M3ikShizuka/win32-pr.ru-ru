---
description: Указывает, имеют ли звуковые потоки в презентации переменную скорость.
ms.assetid: 2bd7eee1-5a93-4bde-8b58-80b6395a094e
title: Атрибут MF_PD_AUDIO_ISVARIABLEBITRATE (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4a34d3dd64f9100050dc9aae37e811d00c9d58af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363925"
---
# <a name="mf_pd_audio_isvariablebitrate-attribute"></a>\_ \_ Атрибут аудиоподсистемы MF PD Audio \_ исвариаблебитрате

Указывает, имеют ли звуковые потоки в презентации переменную скорость.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="applies-to"></a>Применяется к

[**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor)

## <a name="remarks"></a>Remarks

Это необязательный атрибут для дескрипторов представления. Если атрибут имеет **значение true** (не равно нулю), то в презентации содержится по крайней мере один звуковой поток с переменной СКОРОСТЬЮ (VBR). Если атрибут имеет **значение false**, то все звуковые потоки имеют постоянную скорость.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для настольных приложений Server 2008 R2 \|\]<br/>                     |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> </dl>

 

 




