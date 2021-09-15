---
description: Указывает язык для потока.
ms.assetid: b64a9554-a560-4212-8964-b68ebbadc046
title: Атрибут MF_SD_LANGUAGE (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ad13ec4d7d17e715bd2583e499c686de26c7b9da
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572811"
---
# <a name="mf_sd_language-attribute"></a>\_ \_ Атрибут языка MF SD

Указывает язык для потока.

## <a name="data-type"></a>Тип данных

Строка расширенных символов

## <a name="remarks"></a>Комментарии

Значением этого атрибута является тег языка, соответствующий RFC 1766. Этот атрибут применяется к дескрипторам потоков.

Источник мультимедиа (или любой объект, создающий дескриптор потока) может установить этот атрибут, если поток имеет указанный язык. Приложения могут запрашивать этот атрибут для получения языка. Если атрибут не задан, поток не имеет указанного языка.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Приложения UWP для классических приложений Vista \|\]<br/>                              |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для классических приложений сервера 2008 \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: GetString**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getstring)
</dt> <dt>

[**Имфаттрибутес:: SetString**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setstring)
</dt> <dt>

[**имфстреамдескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfstreamdescriptor)
</dt> <dt>

[Атрибуты дескриптора потока](stream-descriptor-attributes.md)
</dt> </dl>

 

 




