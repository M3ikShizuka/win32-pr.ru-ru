---
description: Указывает объект активации, который создает пользовательский Видеомикшер для приемника расширенного модуля подготовки видео (Евр).
ms.assetid: 60484f87-7588-4b52-93aa-ef8fad66d971
title: Атрибут MF_ACTIVATE_CUSTOM_VIDEO_MIXER_ACTIVATE (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9d6268f3630b013235f3d365e0b8ab0578c9dd3e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580426"
---
# <a name="mf_activate_custom_video_mixer_activate-attribute"></a>MF \_ Активация \_ пользовательского \_ \_ микшера \_ активации атрибута

Указывает объект активации, который создает пользовательский Видеомикшер для приемника расширенного модуля подготовки видео (Евр).

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Remarks

При создании Евр с помощью объекта активации этот атрибут можно использовать для установки пользовательского видеомикшера на Евр. Используйте этот атрибут, как показано ниже.

1.  Вызовите функцию [**мфкреатевидеорендерерактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatevideorendereractivate) , чтобы создать объект активации для Евр. Функция возвращает указатель на интерфейс [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) .
2.  Установите этот атрибут для указателя [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) , вызвав [**Имфаттрибутес:: сетункновн**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setunknown). Значение атрибута является указателем на объект активации, реализованный вызывающим объектом. Объект активации вызывающего объекта должен предоставлять интерфейс **имфактивате** .

Если задать этот атрибут, ЕВР вызывает [**имфактивате:: активатеобжект**](/windows/desktop/api/mfobjects/nf-mfobjects-imfactivate-activateobject) для создания пользовательского видеомикшера. Видеомикшер должен предоставлять интерфейс [**имфтрансформ**](/windows/desktop/api/mftransform/nn-mftransform-imftransform) .

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

[Расширенные атрибуты модуля подготовки видео](enhanced-video-renderer-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: неизвестный**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getunknown)
</dt> <dt>

[**Имфаттрибутес:: Сетункновн**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setunknown)
</dt> <dt>

[**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate)
</dt> <dt>

[Объекты активации](activation-objects.md)
</dt> </dl>

 

 




