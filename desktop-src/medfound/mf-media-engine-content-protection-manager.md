---
description: Позволяет модулю мультимедиа воспроизводить защищенное содержимое.
ms.assetid: F6F17EC7-6553-4127-B691-C20C945DD4D8
title: Атрибут MF_MEDIA_ENGINE_CONTENT_PROTECTION_MANAGER (Мфмедиаенгине. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: afb99d1df36c9b9adbf1c099d619df60e1144b87
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127345170"
---
# <a name="mf_media_engine_content_protection_manager-attribute"></a>\_ \_ \_ \_ Атрибут диспетчера защиты содержимого для компонента MF Media Engine \_

Позволяет модулю мультимедиа воспроизводить защищенное содержимое.

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Комментарии

Значение этого атрибута является указателем на интерфейс [**имфконтентпротектионманажер**](/windows/desktop/api/mfidl/nn-mfidl-imfcontentprotectionmanager) . Вызывающий объект должен реализовать интерфейс.

Этот атрибут может быть одним из атрибутов, передаваемых в [**имфмедиаенгинеклассфактори:: CreateInstance**](/windows/desktop/api/mfmediaengine/nf-mfmediaengine-imfmediaengineclassfactory-createinstance). Он необходим, если защищенное содержимое должно воспроизводиться.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ приложения UWP для классических приложений \|\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Мфмедиаенгине. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфмедиаенгинеклассфактори:: CreateInstance**](/windows/desktop/api/mfmediaengine/nf-mfmediaengine-imfmediaengineclassfactory-createinstance)
</dt> </dl>

 

 




