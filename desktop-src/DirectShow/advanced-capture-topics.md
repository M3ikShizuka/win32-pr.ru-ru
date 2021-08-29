---
description: Разделы, посвященные расширенному записи
ms.assetid: 407702b2-5f4f-424d-a3ec-b0473e1b0da3
title: Разделы, посвященные расширенному записи
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8d80ba7615b0ad42bbfe62ae646a4cf7e58897cb678eae836b2b5329eda0e17c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119690514"
---
# <a name="advanced-capture-topics"></a>Разделы, посвященные расширенному записи

В этом разделе описаны некоторые дополнительные аспекты видеозаписи в DirectShow. Большинство проблем, описанных в этом разделе, автоматически обрабатываются интерфейсом [**ICaptureGraphBuilder2**](/windows/desktop/api/Strmif/nn-strmif-icapturegraphbuilder2) . Однако эти сведения могут оказаться полезными, если необходимо устранить неполадки в приложении видеозаписи. Кроме того, этот раздел следует прочесть, если приложение создает собственную диаграмму записи какого-либо типа, и вы обнаружите, что ICaptureGraphBuilder2 не соответствует вашим потребностям. Наконец, в этом разделе содержатся некоторые сведения об использовании фильтра формирователя видео (VMR) в приложении видеозаписи.

Граф видеозаписи можно создать целиком с помощью методов [**играфбуилдер**](/windows/desktop/api/Strmif/nn-strmif-igraphbuilder) . Можно также объединить два интерфейса, используя ICaptureGraphBuilder2 для некоторых задач и Играфбуилдер для других.

В этом разделе рассматриваются следующие вопросы.

-   [Обработка событий перерисовки в видеозаписи](handling-repaint-events-in-video-capture.md)
-   [Работа с категориями ПИН-кодов](working-with-pin-categories.md)
-   [Использование фильтра Smart Tee](using-the-smart-tee-filter.md)
-   [использование наложения Mixer в видеозаписи](using-the-overlay-mixer-in-video-capture.md)
-   [ПИН-коды порта видео](video-port-pins.md)
-   [Тип формата VideoInfo2](videoinfo2-format-type.md)
-   [Создание фильтров Kernel-Mode](creating-kernel-mode-filters.md)
-   [Фильтры драйвера класса WDM](wdm-class-driver-filters.md)
-   [Использование захвата WDDM в DirectShow](using-wddm-capture-in-directshow.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> </dl>

 

 



