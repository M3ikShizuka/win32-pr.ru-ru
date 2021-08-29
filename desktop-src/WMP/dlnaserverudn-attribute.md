---
title: Атрибут Длнасерверудн
description: Атрибут Длнасерверудн — это уникальное имя устройства сервера, на котором размещен элемент мультимедиа.
ms.assetid: 1965731d-1b6e-4d76-a983-fd57c851fcfb
keywords:
- проигрыватель Windows Media атрибута длнасерверудн
topic_type:
- apiref
api_name:
- DLNAServerUDN Attribute
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ec7e88b29f53acf06553b5ff1126d438f67d775f3f7a5341a00b9c19f0199b6b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118997224"
---
# <a name="dlnaserverudn-attribute"></a>Атрибут Длнасерверудн

Атрибут **длнасерверудн** — это уникальное имя устройства сервера, на котором размещен элемент мультимедиа.

## <a name="applies-to"></a>Применяется к

-   [**Звуковые элементы**](audio-item-attributes.md)
-   [**Элементы фото**](photo-item-attributes.md)
-   [**Элементы списка воспроизведения**](playlist-attributes-ref.md)
-   [**Элементы видео**](video-item-attributes.md)

## <a name="remarks"></a>Remarks

Этот атрибут недоступен для элементов мультимедиа в локальной библиотеке текущего пользователя. Он доступен только для элементов мультимедиа, принадлежащих удаленной библиотеке. то есть библиотека, доступная другим пользователям в домашней сети. Чтобы определить, является ли библиотека мультимедиа удаленной, вызовите метод [**ивмплибрари:: Get \_ Type**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmplibrary-get_type).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------|
| Версия<br/> | проигрыватель Windows Media 12<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> </dl>

 

 





