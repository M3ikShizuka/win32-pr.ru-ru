---
description: Идентификаторы GUID для подтипов звука
ms.assetid: c38a1194-e2d8-42ca-8581-4054171f6f44
title: Идентификаторы GUID для подтипов звука
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d26b61dc7c8bb828deb6278b037dd6128afcaf1f
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122483120"
---
# <a name="audio-subtype-guids"></a>Идентификаторы GUID для подтипов звука

Определены следующие идентификаторы GUID для звуковых подтипов. Чтобы указать подтип, задайте атрибут [**\_ \_ подтипа MF MT**](mf-mt-subtype-attribute.md) для типа носителя. За исключением указанных случаев, эти константы определены в файле заголовка мфапи. h.

Если используются эти подтипы, задайте для атрибута " [ \_ \_ основной \_ тип MF MT](mf-mt-major-type-attribute.md) " значение **мфмедиатипе \_ Audio**.




| Идентификатор GUID | Описание | Тег Format (FOURCC) | 
|------|-------------|---------------------|
| <strong>MEDIASUBTYPE_RAW_AAC1</strong> | Расширенное аудио кодирование (AAC).<br /> Этот подтип используется для AAC, содержащихся в AVI-файле, с тегом формата, равным 0x00FF. <br /> Дополнительные сведения см. в разделе <a href="aac-decoder.md"><strong>декодер AAC</strong></a>.<br /> Определено в вмкодекдсп. h<br /> | WAVE_FORMAT_RAW_AAC1 (0x00FF) | 
| <strong>MFAudioFormat_AAC</strong> | Расширенное аудио кодирование (AAC).<br /><blockquote>[!Note]<br />Эквивалентно MEDIASUBTYPE_MPEG_HEAAC, определенному в вмкодекдсп. h.</blockquote><br /> Поток может содержать необработанные данные AAC или AAC данные в потоке передачи звуковых данных (ADTS).<br /> Дополнительные сведения см. в разделе:<br /><ul><li><a href="aac-decoder.md"><strong>Декодер AAC</strong></a></li><li><a href="mpeg-4-file-source.md">Источник файла MPEG-4</a></li></ul> | WAVE_FORMAT_MPEG_HEAAC (0x1610) | 
| <strong>MFAudioFormat_ADTS</strong> | Не используется. | WAVE_FORMAT_MPEG_ADTS_AAC (0x1600) | 
| <strong>MFAudioFormat_ALAC</strong> | Аудиокодек Apple без потерь<br /> поддерживается в Windows 10 и более поздних версиях.<br /> | WAVE_FORMAT_ALAC (0x6C61) | 
| <strong>MFAudioFormat_AMR_NB</strong> | Адаптативе с несколькими скоростями<br /> поддерживается в Windows 8.1 и более поздних версиях.<br /> | WAVE_FORMAT_AMR_NB | 
| <strong>MFAudioFormat_AMR_WB</strong> | Адаптативе Multi-Rate Wideband Audio<br /> поддерживается в Windows 8.1 и более поздних версиях.<br /> | WAVE_FORMAT_AMR_WB | 
| <strong>MFAudioFormat_AMR_WP</strong> | поддерживается в Windows 8.1 и более поздних версиях.<br /> | WAVE_FORMAT_AMR_WP | 
| <strong>MFAudioFormat_Dolby_AC3</strong> | Dolby Digital (AC-3).<br /> То же значение GUID, что и <strong>MEDIASUBTYPE_DOLBY_AC3</strong>, которое определено в ксууидс. h<br /> | Нет. | 
| <strong>MFAudioFormat_Dolby_AC3_SPDIF</strong> | Dolby AC-3 аудио через Sony/Philips Digital Interface (S/PDIF).<br /> Это значение идентификатора GUID идентично приведенным ниже подтипам:<br /><ul><li><strong>KSDATAFORMAT_SUBTYPE_IEC61937_DOLBY_DIGITAL</strong>, определенный в ксмедиа. h.</li><li><strong>MEDIASUBTYPE_DOLBY_AC3_SPDIF</strong>, определенные в UUID. h.</li></ul> | WAVE_FORMAT_DOLBY_AC3_SPDIF (0x0092) | 
| <strong>MFAudioFormat_Dolby_DDPlus</strong> | Dolby Digital Plus.<br /> То же значение GUID, что и <strong>MEDIASUBTYPE_DOLBY_DDPLUS</strong>, которое определено в вмкодекдсп. h.<br /> | None | 
| <strong>MFAudioFormat_DRM</strong> | Зашифрованные звуковые данные, используемые с защищенным звуковым путем. | WAVE_FORMAT_DRM (0x0009) | 
| <strong>MFAudioFormat_DTS</strong> | Звук системы цифрового кинотеатра (DTS). | WAVE_FORMAT_DTS (0x0008) | 
| <strong>MFAudioFormat_FLAC</strong> | Бесплатный аудиокодек без потерь<br /> поддерживается в Windows 10 и более поздних версиях.<br /> | WAVE_FORMAT_FLAC (0xF1AC) | 
| <strong>MFAudioFormat_Float</strong> | Несжатое аудио с плавающей запятой IEEE. | WAVE_FORMAT_IEEE_FLOAT (0x0003) | 
| <strong>MFAudioFormat_Float_SpatialObjects</strong> | Несжатое аудио с плавающей запятой IEEE. | None | 
| <strong>MFAudioFormat_MP3</strong> | Звуковой слой MPEG-3 (MP3). | WAVE_FORMAT_MPEGLAYER3 (0x0055) | 
| <strong>MFAudioFormat_MPEG</strong> | Полезные данные звука MPEG-1. | WAVE_FORMAT_MPEG (0x0050) | 
| <strong>MFAudioFormat_MSP1</strong> | Windows Голосовой кодек Media Audio 9. | WAVE_FORMAT_WMAVOICE9 (0x000A) | 
| <strong>MFAudioFormat_Opus</strong> | Opus<br /> поддерживается в Windows 10 и более поздних версиях.<br /> | WAVE_FORMAT_OPUS (0x704F) | 
| <strong>MFAudioFormat_PCM</strong> | Несжатый звук PCM. | WAVE_FORMAT_PCM (1) | 
| <strong>MFAudioFormat_QCELP</strong> | КЦЕЛП (линейный прогноз для кода Qualcomm). | None | 
| <strong>MFAudioFormat_WMASPDIF</strong> | Windows Media Audio 9 Professional кодек через S/PDIF. | WAVE_FORMAT_WMASPDIF (0x0164) | 
| <strong>MFAudioFormat_WMAudio_Lossless</strong> | Windows кодек мультимедиа media audio 9 без потерь или кодек Windows Media audio 9,1. | WAVE_FORMAT_WMAUDIO_LOSSLESS (0x0163) | 
| <strong>MFAudioFormat_WMAudioV8</strong> | Windows кодек media audio 8, кодек Windows media audio 9 или кодек Windows Media audio 9,1. | WAVE_FORMAT_WMAUDIO2 (0x0161) | 
| <strong>MFAudioFormat_WMAudioV9</strong> | Windows media audio 9 Professional кодек или Windows media audio 9,1 Professional кодека. | WAVE_FORMAT_WMAUDIO3 (0x0162) | 




 

Теги формата, перечисленные в третьем столбце этой таблицы, используются в структуре **вавеформатекс** и определены в файле заголовка ммрег. h.

При наличии тега звукового формата можно создать идентификатор GUID для звукового подтипа следующим образом:

1.  Начните со значения **мфаудиоформат \_ base**, которое определено в мфаф. i.
2.  Замените первый **DWORD** этого GUID тегом Format.

Чтобы определить новую константу GUID, которая следует за этим шаблоном, можно использовать макрос [**define \_ MEDIATYPE \_ GUID**](/windows/desktop/api/mfapi/nf-mfapi-define_mediatype_guid) .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Типы звуковых носителей](audio-media-types.md)
</dt> <dt>

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)
</dt> <dt>

[GUID типа носителя](media-type-guids.md)
</dt> <dt>

[Типы носителей](media-types.md)
</dt> </dl>

 

 




