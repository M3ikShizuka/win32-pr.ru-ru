---
description: Фильтр разделителя потока MPEG-1
ms.assetid: abadf37f-2876-496d-90e7-77c3475a0064
title: Фильтр разделителя потока MPEG-1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6040197fbd04585d9ba04ce87b2780f539bf377f
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122982186"
---
# <a name="mpeg-1-stream-splitter-filter"></a>Фильтр разделителя потока MPEG-1

Этот фильтр разделяет системный поток MPEG-1 в его компонентах аудио-и видеопотоках.




| Метка | Применение |
|--------|-------|
| Интерфейсы фильтра | <a href="/previous-versions/windows/desktop/api/Qnetwork/nn-qnetwork-iammediacontent"><strong>Иаммедиаконтент</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iamstreamselect"><strong>иамстреамселект</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>ибасефилтер</strong></a> | 
| Типы носителей входных закрепления | Основной тип: MEDIATYPE_Stream<br /> Подтипы<br /><ul><li>MEDIASUBTYPE_MPEG1System</li><li>MEDIASUBTYPE_MPEG1VideoCD</li><li>MEDIASUBTYPE_Audio</li><li>MEDIASUBTYPE_Video</li></ul>См. раздел <a href="mpeg-1-media-types.md"> <strong>типы носителей MPEG-1</strong></a><br /> | 
| Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>Имеминпутпин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | 
| Типы носителей для выходного ПИН-кода | Основной тип: MEDIATYPE_Audio или MEDIATYPE_Video<br /> Подтип: MEDIASUBTYPE_MPEG1Payload или MEDIASUBTYPE_MPEG1Packet<br /> См. раздел <a href="mpeg-1-media-types.md"> <strong>типы носителей MPEG-1</strong></a><br /> | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"> <strong>имедиасикинг</strong></a> | 
| Фильтровать CLSID | CLSID_MPEG1Splitter | 
| CLSID страницы свойств | Нет страницы свойств | 
| Исполняемый объект | quartz.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_NORMAL | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Комментарии

Этот файл поддерживает режим Pull только через [**иасинкреадер**](/windows/desktop/api/Strmif/nn-strmif-iasyncreader) . Он не поддерживает режим принудительной отправки.

Так как содержимое MPEG-1 не индексируется, поиск может быть очень приблизительным. Обычно это удобно для фиксированной скорости системного потока MPEG-1 (обычно это оборудование, создаваемое для компакт-диска видео).

Фильтр поддерживает интерфейс [**иаммедиаконтент**](/previous-versions/windows/desktop/api/Qnetwork/nn-qnetwork-iammediacontent) для получения метаданных ID3.

Не все примеры MPEG имеют отметки времени. Отсутствие метки времени в образце MPEG не является ошибкой. Для разработчиков фильтров это означает, что не следует возвращать код ошибки из метода **Receive** входного ПИН-кода, если [**имедиасампле::-Time**](/windows/desktop/api/Strmif/nf-strmif-imediasample-gettime) завершается ошибкой. Если **Receive** возвращает любое значение, отличное от S \_ , это приведет к тому, что разделитель перестанет отправлять образцы.

Если файл содержит поток видео, разделитель потока MPEG-1 поддерживает поиск по номеру кадра. чтобы включить поиск на основе кадров, вызовите [**имедиасикинг:: сеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-settimeformat) в [фильтре Graph Manager](filter-graph-manager.md) с помощью **параметра \_ формат \_ времени** значения.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 




