---
description: Предоставляет интерфейс обратного вызова, который приложение получает объект средства включения содержимого из сеанса защищенного пути к носителю (PMP).
ms.assetid: 66482541-63d4-439b-862f-7507605af5d8
title: Атрибут MF_SESSION_CONTENT_PROTECTION_MANAGER (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c90321ae3c10fd7fa2ec39a4fb478e256291b049
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572787"
---
# <a name="mf_session_content_protection_manager-attribute"></a>\_ \_ \_ Атрибут диспетчера защиты содержимого сеанса MF \_

Предоставляет интерфейс обратного вызова, который приложение получает объект средства включения содержимого из сеанса защищенного пути к носителю (PMP).

## <a name="data-type"></a>Тип данных

**IUnknown\***

## <a name="remarks"></a>Комментарии

Значение этого атрибута является указателем на интерфейс [**имфконтентпротектионманажер**](/windows/desktop/api/mfidl/nn-mfidl-imfcontentprotectionmanager) приложения.

Установите этот атрибут в сеансе PMP с помощью параметра *пконфигуратион* функции [**мфкреатепмпмедиасессион**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatepmpmediasession) .

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

[Атрибуты сеанса мультимедиа](media-session-attributes.md)
</dt> <dt>

[Воспроизведение защищенных файлов мультимедиа](how-to-play-protected-media-files.md)
</dt> </dl>

 

 




