---
description: Указывает время начала для презентаций, помещенных в очередь после первой презентации.
ms.assetid: 087f5d61-b3e6-4fdf-98e6-b018de7b237f
title: Атрибут MF_TOPOLOGY_START_TIME_ON_PRESENTATION_SWITCH (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b5f4c50271ad2da9682be9d259ad855352e844af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363913"
---
# <a name="mf_topology_start_time_on_presentation_switch-attribute"></a>\_ \_ Время начала топологии \_ MF \_ для \_ \_ атрибута переключателя представления

Указывает время начала для презентаций, помещенных в очередь после первой презентации.

## <a name="data-type"></a>Тип данных

**Int64** хранится как **UINT64**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите [**имфаттрибутес:: UInt64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64).

## <a name="applies-to"></a>Применяется к

[**имфтопологи**](/windows/desktop/api/mfidl/nn-mfidl-imftopology)

## <a name="remarks"></a>Remarks

Когда приложение помещает в очередь первый показ в сеансе мультимедиа, приложение задает время начала в параметре *пварстартпоситион* метода [**Имфмедиасессион:: Start**](/windows/desktop/api/mfidl/nf-mfidl-imfmediasession-start) . Однако для всех последующих презентаций время запуска определяется \_ \_ атрибутом времени начала топологии MF в \_ \_ \_ \_ топологии. Время начала указывается в единицах 100-наносекундных относительно начала презентации. Например, если значение равно 50000000, воспроизведение начнется через 5 секунд. Если этот атрибут не задан, время начала по умолчанию равно нулю.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                            |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты топологии](topology-attributes.md)
</dt> </dl>

 

 




