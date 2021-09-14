---
description: Идентификатор CLSID пользовательского средства показа видео для приемника расширенного модуля подготовки видео (Евр).
ms.assetid: f035ee56-7582-45d3-bafe-dd9c821b6326
title: Атрибут MF_ACTIVATE_CUSTOM_VIDEO_PRESENTER_CLSID (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6c0eb913a56671d5d2ac8d27c785e1cc1fbfc51a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460979"
---
# <a name="mf_activate_custom_video_presenter_clsid-attribute"></a>MF \_ активировать \_ настраиваемый \_ \_ \_ атрибут CLSID видеоустройства

Идентификатор CLSID пользовательского средства показа видео для приемника расширенного модуля подготовки видео (Евр).

## <a name="data-type"></a>Тип данных

**GUID**

## <a name="remarks"></a>Remarks

Если вы создаете Евр с помощью объекта активации, этот атрибут можно использовать для задания пользовательского устройства показа видео в Евр. Используйте этот атрибут, как показано ниже.

1.  Вызовите функцию [**мфкреатевидеорендерерактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatevideorendereractivate) , чтобы создать объект активации для Евр. Функция возвращает указатель на интерфейс [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) .

2.  Задайте этот аттрибуе в указателе [**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate) , вызвав [**Имфаттрибутес:: сетгуид**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setguid). Значением атрибута является идентификатор CLSID пользовательского выступающего видео приложения.

Если этот атрибут задан, ЕВР вызывает **CoCreateInstance** с указанным идентификатором CLSID для создания пользовательского устройства показа видео. Устройство показа видео должно предоставлять интерфейс [**имфвидеопресентер**](/windows/desktop/api/evr/nn-evr-imfvideopresenter) . Выступающий создается как внутрипроцессный COM-сервер.

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

[**Имфаттрибутес:: a GUID**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getguid)
</dt> <dt>

[**Имфаттрибутес:: Сетгуид**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setguid)
</dt> <dt>

[**имфактивате**](/windows/desktop/api/mfobjects/nn-mfobjects-imfactivate)
</dt> <dt>

[Объекты активации](activation-objects.md)
</dt> <dt>

[Написание выступающего Евр](how-to-write-an-evr-presenter.md)
</dt> </dl>

 

 




