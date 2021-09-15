---
description: Содержит код ошибки последней ошибки подключения для данного узла топологии.
ms.assetid: fae90e06-0ae0-43a1-aaf2-7a2d1dabc79b
title: Атрибут MF_TOPONODE_ERRORCODE (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4b4b28c8f630d06f3545ca44c5b064c0bb6dac32
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580327"
---
# <a name="mf_toponode_errorcode-attribute"></a>\_ \_ Атрибут ошибки MF топоноде

Содержит код ошибки последней ошибки подключения для данного узла топологии.

## <a name="data-type"></a>Тип данных

**UINT32**

Ттреат как значение **HRESULT** .

## <a name="remarks"></a>Remarks

Этот атрибут применяется ко всем типам узлов.

Значением этого атрибута является значение **HRESULT** .

В сеансе мультимедиа или загрузчике топологии может быть задан атрибут. Приложения обычно считывают этот атрибут, но не устанавливают его.

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

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**имфтопологиноде**](/windows/desktop/api/mfidl/nn-mfidl-imftopologynode)
</dt> <dt>

[Атрибуты узла топологии](topology-node-attributes.md)
</dt> </dl>

 

 




