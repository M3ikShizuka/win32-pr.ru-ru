---
description: Фильтр синтаксического анализатора с несколькими файлами
ms.assetid: 8ef06f49-fda4-49e2-9b07-70453a2e897c
title: Фильтр синтаксического анализатора с несколькими файлами
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 444eebb6ff16b7b6d5568b47c939f687bb3207c8
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122474630"
---
# <a name="multi-file-parser-filter"></a>Фильтр синтаксического анализатора с несколькими файлами

Фильтр синтаксического анализатора с несколькими файлами анализирует простой формат файла, который позволяет указать несколько имен файлов, как если бы они были одним файлом. Эти файлы имеют формат, показанный в следующем примере:


```C++
;MULTI
https://server/share/video.mpg
https://server/share/captions.smi
```



Использование этого фильтра является устаревшим. Для отрисовки нескольких файлов в одном графе фильтра приложение должно просто вызвать **RenderFile** или **аддсаурцефилтер** несколько раз.




| | | Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>Ибасефилтер</strong></a> | | Типы входных закрепления <ul><li>Основной тип: MEDIATYPE_Stream</li><li>Подтип: CLSID_MultFile</li><li>Тип формата: GUID_NULL</li></ul> | | Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | | Типы выходных закрепления <ul><li>Основной тип: MEDIATYPE_File</li><li>Подтип: GUID_NULL</li><li>Тип формата: MEDIATYPE_File</li></ul> | | Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | | Фильтровать CLSID | CLSID_MultFile | | Исполняемый файл | Quartz.dll | | <a href="merit.md"></a> Кому | MERIT_UNLIKELY | | <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Комментарии

Фильтр создает один выходной ПИН-код для каждого файла, указанного в исходном файле. Тип выходных данных — MEDIATYPE \_ File, а блок формата для выходного типа — это строка расширенных символов, содержащая имя файла. Каждый ПИН-код подключается к экземпляру фильтра модуля [подготовки к потоку файлов](file-stream-renderer-filter.md) . Фильтр модуля подготовки к потоку файлов создает один выходной ПИН-код, который предоставляет интерфейс [**истреамбуилдер**](/windows/desktop/api/Strmif/nn-strmif-istreambuilder) . Закрепление вывода подготавливает к просмотру указанный файл. Данные мультимедиа не передаются между средством синтаксического анализа нескольких файлов и модулем подготовки потока файлов.

CLSID фильтра не определен в UUIDs. h. Используйте этот макрос в своем собственном файле заголовка:


```C++
// {D51BD5A3-7548-11cf-A520-0080C77EF58A}
DEFINE_GUID(CLSID_MultFile,
0xd51bd5a3, 0x7548, 0x11cf, 0xa5, 0x20, 0x0, 0x80, 0xc7, 0x7e, 0xf5, 0x8a);
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 



