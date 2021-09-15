---
description: Указывает, отменила ли источник Sequencer топологию.
ms.assetid: b7252336-1612-43fc-8f08-1fdfdbb293eb
title: Атрибут MF_EVENT_SOURCE_TOPOLOGY_CANCELED (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a2a161aec292d834b0418f59f1c26ea2f11a538e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460973"
---
# <a name="mf_event_source_topology_canceled-attribute"></a>\_Атрибут " \_ топология источника события MF \_ \_ отменен"

Указывает, отменила ли [источник Sequencer](sequencer-source.md) топологию.

## <a name="data-type"></a>Тип данных

**UINT32**

Рассматривать как логическое значение.

## <a name="remarks"></a>Remarks

Этот атрибут используется со следующими событиями:

-   [миндофпресентатионсегмент](meendofpresentationsegment.md)
-   [миндофпресентатион](meendofpresentation.md)

Если этот атрибут имеется и имеет ненулевое значение, это означает, что сегмент презентации завершен, так как источник Sequencer отменил топологию. В противном случае сегмент презентации завершается нормально.

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

[Атрибуты событий](event-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[События источника Sequencer](sequencer-source-events.md)
</dt> </dl>

 

 




