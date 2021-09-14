---
description: Содержит указатель на прокси-объект для дескриптора представления приложений.
ms.assetid: 0cd83204-0d32-417c-8911-1d3358eb0802
title: Атрибут MF_PD_PMPHOST_CONTEXT (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 70e8903e438a4649ae43d7aa2072e5a5146e3126
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257792"
---
# <a name="mf_pd_pmphost_context-attribute"></a>\_ \_ Атрибут контекста MF PD пмфост \_

Содержит указатель на прокси-объект для дескриптора представления приложения.

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Комментарии

Узел защищенного пути к носителю (PMP) использует этот атрибут для хранения дескриптора представления приложения в дескрипторе удаленной презентации. Значение атрибута является указателем на интерфейс [**имфремотепрокси**](/windows/desktop/api/mfidl/nn-mfidl-imfremoteproxy) .

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

[**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor)
</dt> <dt>

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> </dl>

 

 




