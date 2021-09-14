---
title: Что нового в проигрывателе Windows Media 11
description: в этом разделе перечислены новые возможности проигрыватель Windows Media 11 и пакета SDK для проигрыватель Windows Media 11.
ms.assetid: d2a6b6ce-a924-4b55-9dc7-68cc57e5651f
keywords:
- проигрыватель Windows Media, новые возможности
- проигрыватель Windows Media, новые функции
- пакет средств разработки программного обеспечения (SDK), проигрыватель Windows Media 11
- пакет SDK (пакет средств разработки программного обеспечения), проигрыватель Windows Media 11
- документация, пакет SDK для проигрыватель Windows Media 11
- новые возможности, проигрыватель Windows Media 11
- новые функции, проигрыватель Windows Media 11
- интерфейсы, новые функции в проигрыватель Windows Media 11
- атрибуты, новые функции в проигрыватель Windows Media 11
- проигрыватель Windows Media ActiveX элемент управления, новые функции в версии 11
- ActiveX элемент управления, новые функции в версии 11
- обложки, новые функции в проигрыватель Windows Media 11
- обложки проигрыватель Windows Media, новые функции в версии 11
- подключаемые модули, новые функции в проигрыватель Windows Media 11
- проигрыватель Windows Media подключаемые модули, новые возможности в версии 11
- интернет-магазины, новые функции в проигрыватель Windows Media 11
- проигрыватель Windows Media интернет-магазинов, новых функций в версии 11
- примеры, новые функции в проигрыватель Windows Media 11
- версии проигрыватель Windows Media, новые функции в версии 11
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 12aa728aa1552ac0e65f5825cad62d8e9e0c7300
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243025"
---
# <a name="what-was-new-in-windows-media-player-11"></a>Что нового в проигрывателе Windows Media 11

в этом разделе перечислены новые возможности проигрыватель Windows Media 11 и пакета SDK для проигрыватель Windows Media 11.

## <a name="windows-media-player-control"></a>проигрыватель Windows Media Элемента

следующие интерфейсы были впервые добавлены в элемент управления ActiveX проигрыватель Windows Media 11.

-   [**Интерфейс Ивмплибрари**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmplibrary)
-   [**Интерфейс Ивмплибрарисервицес**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmplibraryservices)
-   [**Интерфейс Ивмплибраришарингсервицес**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmplibrarysharingservices)
-   [**Интерфейс IWMPMediaCollection2**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpmediacollection2)
-   [**Интерфейс Ивмпкуери**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpquery)
-   [**Интерфейс IWMPStringCollection2**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpstringcollection2)
-   [**Объект Медиаколлектион**](mediacollection-object.md)
-   [**Объект запроса**](query-object.md)
-   [**Объект StringCollection**](stringcollection-object.md)
-   [**Интерфейс Ивмпкдромрип**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpcdromrip)
-   [**Интерфейс Ивмпкдромбурн**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpcdromburn)
-   [**Интерфейс Ивмпфолдермониторсервицес**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpfoldermonitorservices)
-   [**Интерфейс IWMPSyncDevice2**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpsyncdevice2)
-   [**Интерфейс Ивмпвидеорендерконфиг**](/previous-versions/windows/desktop/api/wmprealestate/nn-wmprealestate-iwmpvideorenderconfig)
-   [**ивмпусеревентсинк**](/previous-versions/windows/desktop/api/wmpservices/nn-wmpservices-iwmpusereventsink)
-   [**Интерфейс IWMPEvents3**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpevents3)

## <a name="windows-media-player-skins"></a>проигрыватель Windows Media Палитр

в проигрыватель Windows Media 11 появились следующие функции обложки.

-   Новые атрибуты для позиционирования элементов управления. См. раздел [**амбиентаттрибутес. Right**](ambientattributes-right.md) и [**амбиентаттрибутес. Bottom**](ambientattributes-bottom.md).
-   Новые атрибуты для перемещения и изменения размеров элементов управления. См. раздел [**амбиентаттрибутес. мовесизето**](ambientattributes-movesizeto.md) and [**амбиентаттрибутес. слидето**](ambientattributes-slideto.md).
-   Новый атрибут для указания поведения при изменении размера изображения. См. раздел [**амбиентаттрибутес. ресизеимажес**](ambientattributes-resizeimages.md).
-   Новый атрибут для указания неоднородного масштабирования элемента обложки. См. раздел [**амбиентаттрибутес. нинегридмаргинс**](ambientattributes-ninegridmargins.md).

## <a name="windows-media-player-plug-ins"></a>проигрыватель Windows Media Подключаемые модули

в пакете SDK для проигрыватель Windows Media 11 появился новый тип подключаемого модуля для преобразования форматов цифровых мультимедийных файлов. см. раздел [подключаемые модули преобразования проигрыватель Windows Media](windows-media-player-conversion-plug-ins.md).

подключаемые модули DSP, созданные до выпуска пакета SDK для проигрыватель Windows Media 11, должны быть обновлены для работы с проигрыватель Windows Media 11. См. статью [обновление существующих подключаемых модулей DSP](updating-existing-dsp-plug-ins.md).

мастер подключаемых модулей проигрыватель Windows Media был обновлен, чтобы создать подключаемые модули DSP, работающие в проигрыватель Windows Media 11. дополнительные сведения см. в разделе [обновления мастера подключаемых модулей DSP для проигрыватель Windows Media 11](updates-to-the-dsp-plug-in-wizard-for-windows-media-player-11.md).

## <a name="windows-media-player-online-stores"></a>проигрыватель Windows Media Интернет-магазины

в проигрыватель Windows Media 11 появилась новая модель для интеграции каталогов интернет-магазина в функцию библиотеки проигрыватель Windows Media. См. раздел [Type 1 Online Stores](type-1-online-stores.md).

## <a name="windows-media-player"></a>Проигрыватель Windows Media

следующие возможности появились в проигрыватель Windows Media 11.

-   [Расширения устройств для создания отчетов о приобретенном содержимом](device-extensions-for-reporting-acquired-content.md)
-   [Расширения устройств для параметров объектов списков воспроизведения](device-extensions-for-playlist-object-preferences.md)

## <a name="windows-media-player-sdk-samples"></a>проигрыватель Windows Media Примеры SDK

пример C# с именем счемареадер был впервые добавлен в пакет SDK для проигрыватель Windows Media 11. в примере создается средство, использующее объектную модель проигрыватель Windows Media для получения и просмотра сведений о метаданных в библиотеке проигрыватель Windows Media или в цифровом файле мультимедиа. Средство может сохранить результаты в текстовый файл. Средство перечисляет имена атрибутов метаданных, хранящиеся в библиотеке, для каждой поддерживаемой схемы (аудио, видео, списков воспроизведения, фотографий и т. д.). Средство также может предоставлять сведения о доступных атрибутах для списков воспроизведения в коллекции списков воспроизведения, на компакт-дисках, оглавлении компакт-дисков, на DVD-дисках, в разделах с DVD, оглавлении и отдельных файлах мультимедиа.

пример C++ с именем вмпмл был обновлен в пакете SDK для проигрыватель Windows Media 11, чтобы продемонстрировать следующие возможности:

-   использование нового интерфейса [**IWMPStringCollection2**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpstringcollection2) для создания пользовательского интерфейса, аналогичного функции библиотеки проигрыватель Windows Media.
-   Использование интерфейсов [**ивмпкуери**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpquery) и [**IWMPMediaCollection2**](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpmediacollection2) для создания составных запросов и вывода результатов.

 

 




