---
description: 'В примере кода Реиндексматчингурлс показано, как предоставить три способа указания файлов для повторного индексирования: URL-адреса, соответствующие типу файла, типу MIME или указанному предложению WHERE.'
ms.assetid: f7b3a8a6-b464-46d4-a99c-fc56eea9b1ec
title: реиндексматчингурлс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 08a7bb6ae3148f6969fc5349e1ebdf666a527282
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363237"
---
# <a name="reindexmatchingurls"></a>реиндексматчингурлс

В примере кода Реиндексматчингурлс показано, как предоставить три способа указания файлов для повторного индексирования: URL-адреса, соответствующие типу файла, типу MIME или указанному предложению WHERE.

В этом разделе содержатся следующие подразделы.

- [Requirements](#requirements)
- [Загрузка образца](#downloading-the-sample)
- [Создание примера](#building-the-sample)
- [Запуск примера](#running-the-sample)
- [Связанные темы](#related-topics)

## <a name="requirements"></a>Требования

| Продукт     | Версия продукта          |
|-------------|--------------------------|
| Windows     | Windows 7, 8.1 или 10    |
| Пакет Windows SDK | 7,0 или выше           |

## <a name="downloading-the-sample"></a>Загрузка образца

Этот пример доступен в следующем расположении.

| Расположение      | URL-адрес пути                                                                      |
|---------------|-------------------------------------------------------------------------------|
| GitHub  | [Пример Реиндексматчингурлс](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/WindowsSearch/ReindexMatchingUrls) |

> [!NOTE]  
> для всех версий Windows, включая Windows 7, рекомендуется загружать образцы непосредственно из GitHub для наиболее актуальной версии.

## <a name="building-the-sample"></a>Построение образца

1. откройте обозреватель Windows и перейдите в каталог проекта **реиндексматчингурлс** . Например, полный путь установки по умолчанию — `C:\Program Files\Microsoft SDKs\Windows\v7.0\Samples\WinUI\WindowsSearch\ReindexMatchingUrls` .
2. Дважды щелкните значок для файла reindex. sln, чтобы открыть проект в Visual Studio.
  
    > [!NOTE]  
    > файл sln был создан в более ранней версии Visual Studio, поэтому его обновление потребуется при использовании Visual Studio 2012 или более поздних версий. Это не повлияет на поведение образца.

3. В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1. перейдите в каталог, содержащий новый исполняемый файл, используя окно командной строки или проводник Windows.
2. в командной строке введите `Reindex.exe` или в Windows Explorer дважды щелкните значок Reindex.exe.

## <a name="related-topics"></a>Связанные темы

### <a name="reference"></a>Справочник

[**исеарчкаталогманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager)

[**ISearchCatalogManager2**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager2)

[**исеарчманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchmanager)

[**исеарчперсистентитемсчанжедсинк**](/windows/desktop/api/Searchapi/nn-searchapi-isearchpersistentitemschangedsink)

[**исеарчвиевчанжедсинк**](/windows/desktop/api/searchapi/nn-searchapi-isearchviewchangedsink)

[**определение приоритетов \_ флагов**](/windows/win32/api/searchapi/ne-searchapi-tagprioritize_flags)

### <a name="other-samples"></a>Другие примеры

[Поиск примеров кода](-search-samples-ovw.md)
