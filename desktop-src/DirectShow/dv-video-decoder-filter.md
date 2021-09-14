---
description: Фильтр видеодекодера DV
ms.assetid: aa47010e-8510-475d-836a-cb63deeb3a7b
title: Фильтр видеодекодера DV
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b12aead5f8238064198c31566a1e2ca1fde75931
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246610"
---
# <a name="dv-video-decoder-filter"></a>Фильтр видеодекодера DV

Этот фильтр декодирует поток цифрового видео (DV) в несжатое видео.




| Метка | Значение |
|--------|-------|
| Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>Ибасефилтер</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-idvrgb219"><strong>IDVRGB219</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iipdvdec"><strong>иипдвдек</strong></a>, <strong>IPersistStream</strong>, <strong>испеЦифипропертипажес</strong> | 
| Типы носителей входных закрепления | <ul><li>MEDIATYPE_Video</li><li>MEDIASUBTYPE_dvsd</li><li>FORMAT_VideoInfo, FORMAT_DvInfo</li></ul> | 
| Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>Имеминпутпин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | 
| Типы носителей для выходного ПИН-кода | <strong>Основной тип</strong>: MEDIATYPE_Video<strong>подтипы</strong>:<br /><ul><li>MEDIASUBTYPE_YUY2</li><li>MEDIASUBTYPE_UYVY</li><li>MEDIASUBTYPE_RGB24</li><li>MEDIASUBTYPE_RGB32</li><li>MEDIASUBTYPE_ARGB32</li><li>MEDIASUBTYPE_RGB565</li><li>MEDIASUBTYPE_RGB555</li><li>MEDIASUBTYPE_RGB8</li><li>MEDIASUBTYPE_Y41P</li></ul><strong>Типы форматов</strong>:<br /> Format_VideoInfo, Format_VideoInfo2<br /> | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Control/nn-control-imediaposition"><strong>Имедиапоситион</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"><strong>имедиасикинг</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | 
| Фильтровать CLSID | CLSID_DVVideoCodec | 
| CLSID страницы свойств | CLSID_DVDecPropertiesPage | 
| Исполняемый объект | qdv.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_NORMAL | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Remarks

Используйте интерфейс [**иипдвдек**](/windows/desktop/api/Strmif/nn-strmif-iipdvdec) , чтобы задать разрешение декодирования: полный, половинный размер, квартал или один восьмой размер.

**Чередование**. более ранние версии декодера всегда разменяют чересстрочную развертку видео. Начиная с DirectX 9,0, декодер DV video может сохранить чересстрочную развертку. Это позволяет разрисовать чередование видео с помощью формирователя микширования видео (VMR) для улучшения качества отрисовки. Чтобы использовать эту функцию, нисходящий фильтр должен поддерживать форматы [**VIDEOINFOHEADER2**](/previous-versions/windows/desktop/api/dvdmedia/ns-dvdmedia-videoinfoheader2) , обозначенные этим форматом значения \_ VideoInfo2 в элементе **Форматтипе** структуры [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) . В выходных данных полного разрешения флаги разчередования (**двинтерлаце**) в структуре **VIDEOINFOHEADER2** устанавливаются в значение `AMINTERLACE_IsInterlaced | AMINTERLACE_DisplayModeBobOrWeave` , указывающее на поля с чередованием. В половине разрешения или ниже **двинтерлаце** устанавливается равным нулю, что означает последовательные кадры.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> <dt>

[Цифровое видео в DirectShow](digital-video-in-directshow.md)
</dt> </dl>

 

 




