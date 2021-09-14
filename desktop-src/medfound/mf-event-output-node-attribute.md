---
description: Определяет узел топологии для приемника потока.
ms.assetid: 9aa6ca66-5122-4d05-94b9-32be194e9eb3
title: Атрибут MF_EVENT_OUTPUT_NODE (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 02c484ea55841f4057bf0855dd51b90db951acb6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460974"
---
# <a name="mf_event_output_node-attribute"></a>\_ \_ Атрибут узла вывода события MF \_

Определяет узел топологии для приемника потока.

## <a name="data-type"></a>Тип данных

**UINT64**

Рассматривать как [**топоид**](topoid.md).

## <a name="remarks"></a>Remarks

Значение этого атрибута является идентификатором узла для выходного узла в текущей топологии. Чтобы получить указатель на связанный узел, вызовите [**имфтопологи:: жетнодебид**](/windows/desktop/api/mfidl/nf-mfidl-imftopology-getnodebyid) в топологии.

Этот атрибут используется со следующими событиями:

-   [месессионстреамсинкформатчанжед](mesessionstreamsinkformatchanged.md)
-   [месинкинвалидатед](mesinkinvalidated.md)

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

[**Имфаттрибутес:: UINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64)
</dt> <dt>

[**Имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64)
</dt> </dl>

 

 




