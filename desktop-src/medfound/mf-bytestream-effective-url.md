---
description: Возвращает действующий URL-адрес потока байтов.
ms.assetid: 0A83CFC0-7EAA-464B-BA39-50DF220AF683
title: Атрибут MF_BYTESTREAM_EFFECTIVE_URL (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b95e01238f04c30f72d55f940b3f3105863247ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127364108"
---
# <a name="mf_bytestream_effective_url-attribute"></a>\_Атрибут BYTESTREAM для \_ действующего \_ URL-адреса MF

Возвращает действующий URL-адрес потока байтов.

## <a name="data-type"></a>Тип данных

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: GetString**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getstring).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetString**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setstring).

## <a name="applies-to"></a>Применяется к

[**имфбитестреам**](/windows/desktop/api/mfobjects/nn-mfobjects-imfbytestream)

## <a name="remarks"></a>Remarks

Действующий URL-адрес может отличаться от исходного URL-адреса, если исходный URL-адрес содержит дополнительные сведения, например строки поиска или привязки, или если запрос был перенаправлен.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ приложения UWP для классических приложений \|\]<br/>                            |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты потока байтов](byte-stream-attributes.md)
</dt> <dt>

[**имфбитестреам**](/windows/desktop/api/mfobjects/nn-mfobjects-imfbytestream)
</dt> </dl>

 

 




