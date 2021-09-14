---
description: Смещение между отметкой времени в каждом примере, полученным с помощью образца области захвата, и времени, в котором этот пример представляет образец.
ms.assetid: 8d06b415-aafc-4276-9a88-4b7262df62f1
title: Атрибут MF_SAMPLEGRABBERSINK_SAMPLE_TIME_OFFSET (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d99f65c5023bbe8705e21269dfb07d6f24db4190
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257784"
---
# <a name="mf_samplegrabbersink_sample_time_offset-attribute"></a>\_ \_ \_ Атрибут смещения времени выборки MF самплеграбберсинк \_

Смещение между отметкой времени в каждом примере, полученным с помощью образца области захвата, и времени, в котором этот пример представляет образец.

## <a name="data-type"></a>Тип данных

**UINT64**

## <a name="remarks"></a>Комментарии

Этот атрибут можно задать для объекта [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) , возвращаемого функцией [**мфкреатесамплеграбберсинкактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatesamplegrabbersinkactivate) . Этот атрибут позволяет функции обратного вызова образца захвата получать примеры, предшествующие времени презентации.

Когда образец захвата получает новый пример, он представляет пример на время *t* −, где *t* — это метка времени в *примере, а* *offset* — значение этого атрибута. Если этот атрибут не задан, значение по умолчанию равно нулю.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64)
</dt> <dt>

[**Имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64)
</dt> <dt>

[**имфсамплеграбберсинккаллбакк**](/windows/desktop/api/mfidl/nn-mfidl-imfsamplegrabbersinkcallback)
</dt> <dt>

[Атрибуты Media Foundation](media-foundation-attributes.md)
</dt> </dl>

 

 




