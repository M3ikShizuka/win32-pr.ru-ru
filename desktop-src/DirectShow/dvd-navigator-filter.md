---
description: Фильтр DVD Navigator
ms.assetid: 3b2c01a2-d52c-4497-8fc9-d1113e8507e8
title: Фильтр DVD Navigator
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a48d4978b31683d99035f6e44ae042f3e982bcde
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122983217"
---
# <a name="dvd-navigator-filter"></a>Фильтр DVD Navigator

Фильтр "Навигатор DVD" является фильтром источников для диаграммы фильтра воспроизведения DVD-Video. Он открывает все необходимые файлы в DVD-Video томе, выполняет переходы по линейным DVD-Video. VOB-файлам и анализирует полученный поток программы MPEG-2, разбивая поток на три (видео, аудио, субтитры) выходного контакта.

Фильтр навигатора по DVD также реализует интерфейсы [**IDvdControl2**](/windows/desktop/api/Strmif/nn-strmif-idvdcontrol2) и [**IDvdInfo2**](/windows/desktop/api/Strmif/nn-strmif-idvdinfo2) , позволяющие приложению воспроизведения DVD управлять DVD-Video воспроизведения.




| Метка | Применение |
|--------|-------|
| Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>Ибасефилтер</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-idvdcontrol2"><strong>IDvdControl2</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-idvdinfo2"><strong>IDvdInfo2</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ifilesourcefilter"><strong>ифилесаурцефилтер</strong></a>, <strong>испеЦифипропертипажес</strong> | 
| Типы носителей входных закрепления | MEDIATYPE_Stream, MEDIASUBTYPE_MPEG2_PROGRAM | 
| Интерфейсы входных закрепления | Не применяется | 
| Типы носителей для выходного ПИН-кода | Базовые типы:<br /><ul><li>Видео: <strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_MPEG2_VIDEO</strong></li><li>Аудио: <strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_DOLBY_AC3</strong></li><li>Подизображение: <strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_DVD_SUBPICTURE</strong></li></ul>Расширенные типы:<br /> Видео:<br /><ul><li><strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_MPEG2_VIDEO</strong></li><li><strong>MEDIATYPE_Video</strong>, <strong>MEDIASUBTYPE_MPEG2_VIDEO</strong></li><li><strong>MEDIATYPE_MPEG2_PES</strong>, <strong>MEDIASUBTYPE_MPEG2_VIDEO</strong></li></ul>Звук:<br /><ul><li><strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_DOLBY_AC3</strong></li><li><strong>MEDIATYPE_Audio</strong>, <strong>MEDIASUBTYPE_DOLBY_AC3</strong></li><li><strong>MEDIATYPE_MPEG2_PES</strong>, <strong>MEDIASUBTYPE_DOLBY_AC3</strong></li></ul>Субтитров<br /><ul><li><strong>MEDIATYPE_DVD_ENCRYPTED_PACK</strong>, <strong>MEDIASUBTYPE_DVD_SUBPICTURE</strong></li><li><strong>MEDIATYPE_Video</strong>, <strong>MEDIASUBTYPE_DVD_SUBPICTURE</strong></li><li><strong>MEDIATYPE_MPEG2_PES</strong>, <strong>MEDIASUBTYPE_DVD_SUBPICTURE</strong></li></ul>Чтобы включить расширенные типы, вызовите метод <a href="/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-setoption"><strong>IDvdControl2:: SetOption</strong></a> и установите для свойства <br /> | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"> <strong>икуалитиконтрол</strong></a> | 
| Фильтровать CLSID | CLSID_DVDNavigator | 
| CLSID страницы свойств | Нет страницы свойств. | 
| Исполняемый объект | qdvd.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_DO_NOT_USE | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> <dt>

[DVD-приложения](dvd-applications.md)
</dt> </dl>

 

 




