---
description: Фильтр синтаксического анализатора с несколькими файлами
ms.assetid: 8ef06f49-fda4-49e2-9b07-70453a2e897c
title: Фильтр синтаксического анализатора с несколькими файлами
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8a91196f9712dc05e64f1d70072d3af9d1c0a39f
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122986476"
---
# <a name="multi-file-parser-filter"></a>Фильтр синтаксического анализатора с несколькими файлами

Фильтр синтаксического анализатора с несколькими файлами анализирует простой формат файла, который позволяет указать несколько имен файлов, как если бы они были одним файлом. Эти файлы имеют формат, показанный в следующем примере:


```C++
;MULTI
https://server/share/video.mpg
https://server/share/captions.smi
```



Использование этого фильтра является устаревшим. Для отрисовки нескольких файлов в одном графе фильтра приложение должно просто вызвать **RenderFile** или **аддсаурцефилтер** несколько раз.




| Метка | Применение |
|--------|-------|
| Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>ибасефилтер</strong></a> | 
| Типы носителей входных закрепления | <ul><li>Основной тип: MEDIATYPE_Stream</li><li>Подтип: CLSID_MultFile</li><li>Тип формата: GUID_NULL</li></ul> | 
| Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"> <strong>икуалитиконтрол</strong></a> | 
| Типы носителей для выходного ПИН-кода | <ul><li>Основной тип: MEDIATYPE_File</li><li>Подтип: GUID_NULL</li><li>Тип формата: MEDIATYPE_File</li></ul> | 
| Интерфейсы выходного ПИН-кода | <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"> <strong>икуалитиконтрол</strong></a> | 
| Фильтровать CLSID | CLSID_MultFile | 
| Исполняемый объект | Quartz.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_UNLIKELY | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

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

 

 



