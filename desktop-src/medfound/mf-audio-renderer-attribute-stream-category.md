---
description: Указывает категорию звукового потока для модуля подготовки потоковой передачи звука (САР).
ms.assetid: 88E79DE6-2062-4471-A939-D1D4DD2EC42D
title: Атрибут MF_AUDIO_RENDERER_ATTRIBUTE_STREAM_CATEGORY (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cd96c219e43f85c516a5f862e2a978724328a69f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462189"
---
# <a name="mf_audio_renderer_attribute_stream_category-attribute"></a>\_ \_ \_ \_ Атрибут категории потока атрибута для модуля подготовки звука MF \_

Указывает категорию звукового потока для модуля [подготовки потоковой передачи звука](streaming-audio-renderer.md) (САР).

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Этот атрибут можно использовать для настройки модуля подготовки звука. Использование зависит от того, какая функция вызывается для создания модуля подготовки звука.



| Функция                                                               | Как задать атрибут                                                                                                                                                                       |
|------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**мфкреатеаудиорендерер**](/windows/desktop/api/mfidl/nf-mfidl-mfcreateaudiorenderer)                 | Используйте указатель [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) , указанный в параметре *паудиоаттрибутес* .                                                                                          |
| [**мфкреатеаудиорендерерактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreateaudiorendereractivate) | Используйте указатель [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) , возвращенный в параметре *ппактивате* . Задайте атрибут перед вызовом [**имфактивате:: активатеобжект**](/windows/desktop/api/mfobjects/nf-mfobjects-imfactivate-activateobject). |



 

Значение атрибута является членом перечисления [**\_ \_ категории аудиопотока**](/windows/win32/api/audiosessiontypes/ne-audiosessiontypes-audio_stream_category) . Служба аудио использует категорию Stream для определения политик аудио, когда несколько приложений одновременно воспроизводят звук.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> </dl>

 

 
