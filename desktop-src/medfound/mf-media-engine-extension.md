---
description: Содержит указатель на интерфейс Имфмедиаенгиникстенсион.
ms.assetid: D2F3F41D-086A-4DEB-99D0-07574BC8F0D7
title: Атрибут MF_MEDIA_ENGINE_EXTENSION (Мфмедиаенгине. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4496b40e9b69091b588ad38ad47d943dce5e1966
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127345659"
---
# <a name="mf_media_engine_extension-attribute"></a>\_ \_ Атрибут расширения обработчика мультимедиа MF \_

Содержит указатель на интерфейс [**имфмедиаенгиникстенсион**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediaengineextension) .

## <a name="data-type"></a>Тип данных

**Имфмедиаенгиникстенсион \* *_ хранится как _* IUnknown\***

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите [**имфаттрибутес:: ununknown**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getunknown).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: сетункновн**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setunknown).

## <a name="remarks"></a>Remarks

Этот атрибут используется с методом [**имфмедиаенгинеклассфактори:: CreateInstance**](/windows/desktop/api/mfmediaengine/nf-mfmediaengine-imfmediaengineclassfactory-createinstance) для инициализации механизма мультимедиа.

Этот атрибут является необязательным. Используйте его для предоставления объекта, реализующего интерфейс [**имфмедиаенгиникстенсион**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediaengineextension) . Этот интерфейс позволяет приложению загружать пользовательские ресурсы мультимедиа.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ приложения UWP для классических приложений \|\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Мфмедиаенгине. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> </dl>

 

 




