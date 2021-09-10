---
title: Справочник по диспетчеру сжатия видео
description: Справочник по диспетчеру сжатия видео
ms.assetid: dd678b24-62af-495f-bdd6-3082c1a753dd
keywords:
- видео для Windows (VFW), диспетчер сжатия видео (вкм)
- VFW (видео для Windows), диспетчер сжатия видео (вкм)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c801df7ecdf0f6468762c2742235d4ef627f5aee
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370410"
---
# <a name="video-compression-manager-reference"></a>Справочник по диспетчеру сжатия видео

В этом разделе описываются функции, структуры, сообщения и макросы, связанные с ВКМ. Эти элементы группируются следующим образом.

## <a name="compressor-installation-and-removal"></a>Установка и удаление программы сжатия

-   [**иЦинсталл**](/windows/desktop/api/Vfw/nf-vfw-icinstall)
-   [**иклокате**](/windows/desktop/api/Vfw/nf-vfw-iclocate)
-   [**икопен**](/windows/desktop/api/Vfw/ns-vfw-icopen)
-   [**икклосе**](/windows/desktop/api/Vfw/nf-vfw-icclose)
-   [**икремове**](/windows/desktop/api/Vfw/nf-vfw-icremove)
-   [**икопенфунктион**](/windows/desktop/api/Vfw/nf-vfw-icopenfunction)

## <a name="locating-and-opening-a-compressor"></a>Поиск и открытие программы сжатия

-   [**иклокате**](/windows/desktop/api/Vfw/nf-vfw-iclocate)
-   [**икопен**](/windows/desktop/api/Vfw/ns-vfw-icopen)
-   [**икдекомпрессопен**](/windows/desktop/api/Vfw/nf-vfw-icdecompressopen)
-   [**икдравопен**](/windows/desktop/api/Vfw/nf-vfw-icdrawopen)
-   [**иЦинфо**](/windows/desktop/api/Vfw/ns-vfw-icinfo)
-   [**икклосе**](/windows/desktop/api/Vfw/nf-vfw-icclose)

## <a name="selecting-compressors"></a>Выбор сжатия

-   [**иккомпрессорчусе**](/windows/desktop/api/Vfw/nf-vfw-iccompressorchoose)
-   [**иккомпрессорфри**](/windows/desktop/api/Vfw/nf-vfw-iccompressorfree)
-   [**компварс**](/windows/desktop/api/Vfw/ns-vfw-compvars)

## <a name="configuring-compressors"></a>Настройка компрессоров

-   [**\_Настройка ICM**](icm-configure.md)
-   [**ICM — \_ состояние**](icm-getstate.md)
-   [**ICM \_ SETSTATE**](icm-setstate.md)
-   [**иксендмессаже**](/windows/desktop/api/Vfw/nf-vfw-icsendmessage)

## <a name="compressor-information"></a>Сведения о компрессоре

-   [**икжетинфо**](/windows/desktop/api/Vfw/nf-vfw-icgetinfo)
-   [**иЦинфо**](/windows/desktop/api/Vfw/ns-vfw-icinfo)
-   [**ICM \_ жетдефаулткэйфрамерате**](icm-getdefaultkeyframerate.md)
-   [**икжетдисплайформат**](/windows/desktop/api/Vfw/nf-vfw-icgetdisplayformat)
-   [**ICM \_ жетдефаулткуалити**](icm-getdefaultquality.md)
-   [**ICM \_ о**](icm-about.md)

## <a name="single-image-compression"></a>Сжатие одного образа

-   [**иЦимажекомпресс**](/windows/desktop/api/Vfw/nf-vfw-icimagecompress)

## <a name="sequence-compression"></a>Сжатие последовательностей

-   [**иксеккомпрессфраме**](/windows/desktop/api/Vfw/nf-vfw-icseqcompressframe)
-   [**иксеккомпрессфраместарт**](/windows/desktop/api/Vfw/nf-vfw-icseqcompressframestart)
-   [**иксеккомпрессфраминд**](/windows/desktop/api/Vfw/nf-vfw-icseqcompressframeend)

## <a name="compvars"></a>компварс

-   [**иккомпрессорчусе**](/windows/desktop/api/Vfw/nf-vfw-iccompressorchoose)

## <a name="image-data-compression"></a>Сжатие данных изображения

-   [**иккомпресс**](/windows/desktop/api/Vfw/ns-vfw-iccompress)
-   [**\_ \_ \_ формат получения формата ICM**](icm-compress-get-format.md)
-   [**\_запрос СЖАТИЯ \_ ICM**](icm-compress-query.md)
-   [**\_сжатие для \_ получения \_ размера ICM**](icm-compress-get-size.md)
-   [**\_Начало СЖАТИЯ \_ ICM**](icm-compress-begin.md)
-   [**\_ \_ Окончание сжатия ICM**](icm-compress-end.md)

## <a name="compressor-monitoring"></a>Мониторинг сжатия

-   [**иксетстатуспрок**](/windows/desktop/api/Vfw/ns-vfw-icsetstatusproc)

## <a name="decompressing-single-images"></a>Распаковка отдельных образов

-   [**иЦимажедекомпресс**](/windows/desktop/api/Vfw/nf-vfw-icimagedecompress)

## <a name="decompressing-image-data"></a>Распаковка данных изображения

-   [**икдекомпрессекс**](/windows/desktop/api/Vfw/ns-vfw-icdecompressex)
-   [**икдекомпрессексбегин**](/windows/desktop/api/Vfw/nf-vfw-icdecompressexbegin)
-   [**\_ДЕКОМПРЕССЕКС ICM \_**](icm-decompressex-end.md)
-   [**\_ \_ Получение формата для РАСПАКОВКи ICM \_**](icm-decompress-get-format.md)
-   [**\_ \_ извлечь ПАЛИТРУ ICM распаковки \_**](icm-decompress-get-palette.md)
-   [**икдекомпрессекскуери**](/windows/desktop/api/Vfw/nf-vfw-icdecompressexquery)
-   [**икдекомпресс**](/windows/desktop/api/Vfw/ns-vfw-icdecompress)
-   [**\_Начало распаковки \_ ICM**](icm-decompress-begin.md)
-   [**\_Окончание распаковки ICM \_**](icm-decompress-end.md)
-   [**\_распаковать \_ запрос ICM**](icm-decompress-query.md)

## <a name="using-hardware-drawing-capabilities"></a>Использование Hardware-Drawing возможностей

-   [**икжетинфо**](/windows/desktop/api/Vfw/nf-vfw-icgetinfo)
-   [**икдравбегин**](/windows/desktop/api/Vfw/ns-vfw-icdrawbegin)
-   [**\_Окончание прорисовки ICM \_**](icm-draw-end.md)
-   [**\_Вывод на \_ диск с ICM**](icm-draw-flush.md)
-   [**\_запрос ICM Draw \_**](icm-draw-query.md)
-   [**икдравсугжестформат**](/windows/desktop/api/Vfw/nf-vfw-icdrawsuggestformat)
-   [**\_Начало прорисовки ICM \_**](icm-draw-start.md)
-   [**\_Завершение прорисовки ICM \_**](icm-draw-stop.md)
-   [**ICM \_ жетбуфферсвантед**](icm-getbufferswanted.md)
-   [**\_выясняется прорисовка ICM \_**](icm-draw-realize.md)
-   [**икдравопен**](/windows/desktop/api/Vfw/nf-vfw-icdrawopen)
-   [**икдрав**](/windows/desktop/api/Vfw/ns-vfw-icdraw)
-   [**\_время прорисовки ICM \_**](icm-draw-gettime.md)
-   [**ICM \_ Draw \_ SETTIME**](icm-draw-settime.md)
-   [**\_окно вырисовки ICM \_**](icm-draw-window.md)
-   [**\_выясняется прорисовка ICM \_**](icm-draw-realize.md)
-   [**ICM \_ Draw \_ чанжепалетте**](icm-draw-changepalette.md)
-   [**ICM \_ Draw \_ рендербуффер**](icm-draw-renderbuffer.md)

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Диспетчер сжатия видео](video-compression-manager.md)
</dt> </dl>

 

 




