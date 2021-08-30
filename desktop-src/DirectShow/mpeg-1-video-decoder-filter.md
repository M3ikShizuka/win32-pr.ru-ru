---
description: Фильтр видеодекодера MPEG-1
ms.assetid: 272d2f31-6e57-4ce5-ac86-b4d47f661fea
title: Фильтр видеодекодера MPEG-1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e5dc10284b7f0c75ce408c39dbcea642e9423d76
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122982167"
---
# <a name="mpeg-1-video-decoder-filter"></a>Фильтр видеодекодера MPEG-1

Декодирует видео MPEG-1.




| Метка | Применение |
|--------|-------|
| Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>Ибасефилтер</strong></a>, <strong>испеЦифипропертипажес</strong> | 
| Типы носителей входных закрепления | MEDIATYPE_Video, FORMAT_MPEGVideo<br /> Допустимы следующие подтипы:<br /><ul><li><strong>MEDIASUBTYPE_MPEG1Packet</strong></li><li><strong>MEDIASUBTYPE_MPEG1Payload</strong></li></ul> | 
| Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"> <strong>имеминпутпин</strong></a> | 
| Типы носителей для выходного ПИН-кода | Основной тип: <strong>MEDIATYPE_Video</strong>,<br /> Тип формата: <strong>FORMAT_VideoInfo</strong> или <strong>FORMAT_VideoInfo2</strong><br /> Подтипы<br /><ul><li><strong>MEDIASUBTYPE_RGB24</strong></li><li><strong>MEDIASUBTYPE_RGB32</strong></li><li><strong>MEDIASUBTYPE_RGB8</strong></li><li><strong>MEDIASUBTYPE_RGB555</strong></li><li><strong>MEDIASUBTYPE_RGB565</strong></li><li><strong>MEDIASUBTYPE_UYVY</strong></li><li><strong>MEDIASUBTYPE_Y41P</strong></li><li><strong>MEDIASUBTYPE_YUY2</strong></li></ul> | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"> <strong>икуалитиконтрол</strong></a> | 
| Фильтровать CLSID | <strong>CLSID_CMpegVideoCodec</strong> | 
| CLSID страницы свойств | <strong>CLSID_MpegVideoDecodePropertyPage</strong> | 
| Исполняемый объект | quartz.dll | 
| <a href="merit.md">Заслуживают</a> | 0x40000001 | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Комментарии

Этот фильтр может декодировать в поверхность DirectDraw. Фильтр использует технологию MMX, если компьютер поддерживает технологию MMX.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 




