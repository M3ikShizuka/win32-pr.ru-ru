---
description: Фильтр VGA 16 с оттенокм
ms.assetid: 0a5f4e92-e703-4487-91b0-15265744004e
title: Фильтр VGA 16 с оттенокм
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 36aed289a800a992bc061dc9822209bf4c2b5133647d995dfb675c7d5523bd76
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119071948"
---
# <a name="vga-16-color-ditherer-filter"></a>Фильтр VGA 16 с оттенокм

Фильтр VGA 16, отменяющий цвет, выполняет преобразование из типа цвета RGB в 4-разрядный цвет, чтобы видеопотоки AVI и MPEG могли отображаться на старых 16 цветных мониторах. Этот фильтр вставляется в граф между фильтром декомпрессора и фильтром модуля подготовки видео.



| Метка | Значение |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Интерфейсы фильтра                        | [**ибасефилтер**](/windows/desktop/api/Strmif/nn-strmif-ibasefilter)                                                                                                                 |
| Типы носителей входных закрепления                    | МУЛЬТИМЕДИЙное \_ видео, медиасубтипе \_ RGB8                                                                                                               |
| Интерфейсы входных закрепления                     | [**Имеминпутпин**](/windows/desktop/api/Strmif/nn-strmif-imeminputpin), [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin), [**икуалитиконтрол**](/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol)                                             |
| Типы носителей для выходного ПИН-кода                   | МУЛЬТИМЕДИЙное \_ видео, медиасубтипе \_ RGB4                                                                                                               |
| Интерфейсы выходного ПИН-кода                    | [**Имедиапоситион**](/windows/desktop/api/Control/nn-control-imediaposition), [**имедиасикинг**](/windows/desktop/api/Strmif/nn-strmif-imediaseeking), [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin), [**икуалитиконтрол**](/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol) |
| Фильтровать CLSID                             | \_ДИЗЕРИНГ CLSID                                                                                                                                      |
| CLSID страницы свойств                      | Нет страницы свойств.                                                                                                                                  |
| Исполняемый объект                               | quartz.dll                                                                                                                                         |
| [Заслуживают](merit.md)                       | \_маловероятно                                                                                                                                    |
| [Категория фильтра](filter-categories.md) | \_ЛЕГАЦИАМФИЛТЕРКАТЕГОРИ CLSID                                                                                                                      |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 



