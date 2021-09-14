---
description: Фильтр распаковки AVI
ms.assetid: 6a9914db-483a-429c-9b26-9451578951c9
title: Фильтр распаковки AVI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 214ccfeee18a01fa9c8d52ffbf4593b9de5664bb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127148109"
---
# <a name="avi-decompressor-filter"></a>Фильтр распаковки AVI

Фильтр распаковки AVI включает кодеки (ВКМ) для подключения к графу фильтра. Приложению не нужно добавлять фильтр к графу фильтра; он автоматически извлекается при необходимости фильтром Graph Manager.

когда диспетчер Graph фильтра создает граф для отображения AVI-файла, он проверяет значение FOURCC в заголовке avi файла, чтобы определить, сжимается ли видео-поток. если это так, фильтр Graph Manager добавляет распаковку AVI, которая затем ищет в реестре установленный декомпрессор, который может работать с этим файлом.

> [!Note]  
> декомпрессоры MPEG никогда не реализуются как кодеки вкм, но только как собственные фильтры DirectShow.

 

В своем вышестоящем ПИН-коде сжатие AVI обычно подключается к [разделителю AVI](avi-splitter-filter.md). При закреплении на выходе он обычно подключается к модулю [прорисовки видео](video-renderer-filter.md) или [фильтру мультиплексора AVI](avi-mux-filter.md).



| Метка | Значение |
|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Интерфейсы фильтра                        | [**ибасефилтер**](/windows/desktop/api/Strmif/nn-strmif-ibasefilter)                                                                                                                                                                                 |
| Типы носителей входных закрепления                    | Основной тип: MEDIATYPE \_ видеосубтипе: должен соответствовать коду FourCC для типа сжатия. Дополнительные сведения см. в разделе [Коды FOURCC](fourcc-codes.md).<br/> Тип формата: формат \_ видеоинфо<br/> |
| Интерфейсы входных закрепления                     | [**Имеминпутпин**](/windows/desktop/api/Strmif/nn-strmif-imeminputpin), [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin), [**икуалитиконтрол**](/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol)                                                                                                             |
| Типы носителей для выходного ПИН-кода                   | \_Устройство MEDIATYPE, медиасубтипе \_ null, Format \_ видеоинфо                                                                                                                                                            |
| Интерфейсы выходного ПИН-кода                    | [**Имедиапоситион**](/windows/desktop/api/Control/nn-control-imediaposition), [**имедиасикинг**](/windows/desktop/api/Strmif/nn-strmif-imediaseeking), [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin), [**икуалитиконтрол**](/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol)                                                                 |
| Фильтровать CLSID                             | \_АВИДЕК CLSID                                                                                                                                                                                                      |
| CLSID страницы свойств                      | Нет страницы свойств.                                                                                                                                                                                                  |
| Исполняемый объект                               | quartz.dll                                                                                                                                                                                                         |
| [Заслуживают](merit.md)                       | неуспешный \_ режим                                                                                                                                                                                                      |
| [Категория фильтра](filter-categories.md) | \_ЛЕГАЦИАМФИЛТЕРКАТЕГОРИ CLSID                                                                                                                                                                                      |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 




