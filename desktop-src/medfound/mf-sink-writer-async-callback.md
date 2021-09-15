---
description: Содержит указатель на интерфейс обратного вызова приложений для модуля записи приемника.
ms.assetid: 22df1fa0-469d-4501-aaf0-a0379b7ed096
title: Атрибут MF_SINK_WRITER_ASYNC_CALLBACK (Мфреадврите. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0f11bed051df9107ca3a2247b6c3d0cf2058224c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462080"
---
# <a name="mf_sink_writer_async_callback-attribute"></a>\_ \_ \_ Атрибут асинхронного \_ обратного вызова для записи MF SINK

Содержит указатель на интерфейс обратного вызова приложения для модуля записи приемника.

## <a name="data-type"></a>Тип данных

**[**Имфсинквритеркаллбакк**](/windows/desktop/api/mfreadwrite/nn-mfreadwrite-imfsinkwritercallback) \* *_ хранится как _* IUnknown\***

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите [**имфаттрибутес:: ununknown**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getunknown).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: сетункновн**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setunknown).

## <a name="remarks"></a>Remarks

Значение этого атрибута является указателем на интерфейс [**имфсинквритеркаллбакк**](/windows/desktop/api/mfreadwrite/nn-mfreadwrite-imfsinkwritercallback) приложения.

Используйте этот атрибут со следующими функциями:

-   [**мфкреатесинквритерфроммедиасинк**](/windows/desktop/api/mfreadwrite/nf-mfreadwrite-mfcreatesinkwriterfrommediasink)
-   [**мфкреатесинквритерфромурл**](/windows/desktop/api/mfreadwrite/nf-mfreadwrite-mfcreatesinkwriterfromurl)

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для настольных приложений Server 2008 R2 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Мфреадврите. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты модуля записи приемника](sink-writer-attributes.md)
</dt> </dl>

 

 




