---
description: Содержит указатель на дескриптор представления для источника мультимедиа.
ms.assetid: 4f2c1ad8-fda9-482f-b82a-9838d15d2785
title: Атрибут MF_TOPONODE_PRESENTATION_DESCRIPTOR (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e0d95fae4f2c4d4a482c2a62d57e0835ea4f1c36
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572771"
---
# <a name="mf_toponode_presentation_descriptor-attribute"></a>\_ \_ \_ Атрибут дескриптора представления MF топоноде

Содержит указатель на дескриптор представления для источника мультимедиа.

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Комментарии

Этот атрибут применяется к исходным узлам **( \_ \_ \_ узел топологии MF саурцестреам**).

Значение атрибута является указателем на интерфейс [**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor) дескриптора представления. Атрибут обязателен.

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

[**Имфаттрибутес:: неизвестный**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getunknown)
</dt> <dt>

[**Имфаттрибутес:: Сетункновн**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setunknown)
</dt> <dt>

[**имфтопологиноде**](/windows/desktop/api/mfidl/nn-mfidl-imftopologynode)
</dt> <dt>

[Атрибуты Media Foundation](media-foundation-attributes.md)
</dt> </dl>

 

 




