---
description: Содержит указатель на дескриптор представления из защищенного пути к носителю (PMP).
ms.assetid: cf12552e-0963-46fa-9a26-44dd601ab68c
title: Атрибут MF_PD_APP_CONTEXT (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8971ead121407ff1a7793c16b14f6b02d3dd102e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127345646"
---
# <a name="mf_pd_app_context-attribute"></a>\_ \_ Атрибут контекста приложения MF PD \_

Содержит указатель на дескриптор представления из защищенного пути к носителю (PMP).

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Remarks

Прокси-сервер источника мультимедиа, созданный в процессе PMP, использует этот атрибут для хранения дескриптора удаленной презентации в дескрипторе представления приложения.

Значение этого атрибута является указателем на интерфейс [**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor) .

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

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> </dl>

 

 




