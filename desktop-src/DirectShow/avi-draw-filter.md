---
description: Фильтр рисования AVI
ms.assetid: 86cd8e48-7cfa-46e4-b8f4-609b4d09fe80
title: Фильтр рисования AVI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 44eb62bd686d0604f6a0c4966fa8af4a4ad0d69d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127148106"
---
# <a name="avi-draw-filter"></a>Фильтр рисования AVI

Фильтр рисования AVI автоматически извлекается в граф воспроизведения вместо [распаковки AVI](avi-decompressor-filter.md) при выводе видео во внешний монитор телевизора NTSC.




| Метка | Значение |
|--------|-------|
| Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>ибасефилтер</strong></a> | 
| Типы носителей входных закрепления | Основной тип: MEDIATYPE_VideoSubtypes:<br /><ul><li>MEDIASUBTYPE_MJPG</li><li>MEDIASUBTYPE_TVMJ</li><li>MEDIASUBTYPE_WAKE</li><li>MEDIASUBTYPE_CFCC</li><li>MEDIASUBTYPE_IJPG</li><li>MEDIASUBTYPE_Plum</li><li>MEDIASUBTYPE_DVCS</li><li>MEDIASUBTYPE_DVSD</li><li>MEDIASUBTYPE_MDVF</li><li>Тип формата: FORMAT_VideoInfo</li></ul> | 
| Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>Имеминпутпин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | 
| Типы носителей для выходного ПИН-кода | MEDIATYPE_Video, MEDIASUBTYPE_NULL | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Control/nn-control-imediaposition"><strong>Имедиапоситион</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"><strong>имедиасикинг</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ioverlaynotify"><strong>иоверлайнотифи</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | 
| Фильтровать CLSID | CLSID_AVIDraw | 
| CLSID страницы свойств | Нет страницы свойств. | 
| Исполняемый объект | quartz.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_NORMAL + 100 | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Remarks

Поскольку фильтр рисования AVI и [фильтр записи VFW](vfw-capture-filter.md) подключаются к одному и тому же оборудованию, они не могут находиться в одном графе фильтра.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 




