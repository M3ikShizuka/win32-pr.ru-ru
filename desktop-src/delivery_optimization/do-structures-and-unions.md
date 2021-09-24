---
title: Структуры и объединения оптимизации доставки
description: Интерфейсы оптимизации доставки используют следующие структуры.
ms.assetid: 58A5361E-871A-4911-85BD-83F18CB9A2F5
ms.topic: article
ms.date: 07/03/2019
ms.openlocfilehash: 035b465d61cfcee78a20fda0d275e1eece1a78c5
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520484"
---
# <a name="delivery-optimization-structures-and-unions"></a>Структуры и объединения оптимизации доставки

[Интерфейсы](do-interfaces.md) оптимизации доставки используют следующие структуры.

## <a name="in-this-section"></a>В этом разделе

| Раздел | Описание |
|-|-|
| [**BG_FILE_PROGRESS**](bg-file-progress.md) | Структура **BG_FILE_PROGRESS** предоставляет сведения о ходе выполнения, связанные с файлами, например число переданных байтов. |
| [**BG_FILE_RANGE**](bg-file-range.md) | Структура **BG_FILE_RANGE** определяет диапазон байтов для загрузки из файла. |
| [**BG_JOB_PROGRESS**](bg-job-progress.md) | Структура **BG_JOB_PROGRESS** предоставляет сведения о ходе выполнения, связанные с заданиями, такие как число переданных байтов и файлов. Для заданий отправки это состояние применяется к файлу отправки, а не к файлу ответов.  |
| [**BG_JOB_TIMES**](bg-job-times.md) | Структура **BG_JOB_TIMES** предоставляет штампы времени, связанные с заданием. |
| [**BITS_FILE_PROPERTY_VALUE**](bits-file-property-value.md) | **BITS_FILE_PROPERTY_VALUE** Union предоставляет значение свойства файла оптимизации доставки на основе значения перечисления [**BITS_FILE_PROPERTY_ID**](bits-file-property-id-.md) . |
| [**BITS_JOB_PROPERTY_VALUE**](bits-job-property-value-.md) | **BITS_JOB_PROPERTY_VALUE** Union предоставляет значение свойства задания оптимизации доставки на основе значения перечисления [**BITS_JOB_PROPERTY_ID**](bits-job-property-id.md) . |
| [**DO_DOWNLOAD_ENUM_CATEGORY**](./do/ns-do-do_download_enum_category.md) | Используется **идоманажер:: енумдовнлоадс** для фильтрации перечисления Downloads по значению конкретного свойства. |
| [**DO_DOWNLOAD_RANGE**](./deliveryoptimizationdownloadtypes/ns-deliveryoptimizationdownloadtypes-do_download_range.md) | Определяет один диапазон байтов для скачивания из файла. |
| [**DO_DOWNLOAD_RANGE_INFO**](./do/ns-do-do_download_range_info.md) | Определяет массив диапазонов байтов для скачивания из файла. |
| [**DO_DOWNLOAD_STATUS**](./do/ns-do-do_download_status.md) | Используется для получения состояния определенного скачивания. |
| [**досвармстатс**](doswarmstats.md) | Содержит поля для загрузки и передачи статистики для файла. |