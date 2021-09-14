---
description: Контакты порта видео в записи файлов
ms.assetid: 0fa6d88e-3c64-487f-b007-8c65bf47211d
title: Контакты порта видео в записи файлов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f2361c5a7cdaa7640ece9724000963f39f3f77ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272912"
---
# <a name="video-port-pins-in-file-capture"></a>Контакты порта видео в записи файлов

Если устройство записи имеет порт видео, то ПИН-код видеопорта должен быть подключен к модулю обработки видео, даже если требуется только запись в файл.

если вы вызываете [**ICaptureGraphBuilder2:: RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) со значением **\_ \_ запись категории пин-кода** , а устройство имеет пин-код видеопорта, Graph построитель записи автоматически подключает пин-код видеопорта к [наложение Mixer](overlay-mixer-filter.md) фильтр и подключает Mixer наложения к модулю визуализации видео. построитель Graph захвата скрывает окно видео, вызывая [**ивидеовиндов::p ut \_ автоотображения**](/windows/desktop/api/Control/nf-control-ivideowindow-put_autoshow) со значением **оафалсе**. если позже приложение вызывает **RenderStream** с **\_ \_ предварительной версией категории пин-кода**, для отображения видеоокна в построителе Graph построитель вызовов **поместит функцию \_ автоотображения** со значением **оатруе**.

после вызова **RenderStream** с **\_ \_ захватом категории пин-кода** можно проверить, добавлен ли модуль подготовки видео, выполнив запрос фильтра Graph Manager для интерфейса [**ивидеовиндов**](/windows/desktop/api/Control/nn-control-ivideowindow) .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Запись видео в файл](capturing-video-to-a-file.md)
</dt> </dl>

 

 



