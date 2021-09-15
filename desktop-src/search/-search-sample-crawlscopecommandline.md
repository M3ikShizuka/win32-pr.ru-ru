---
description: В образце кода Кравлскопекоммандлине показано, как определить параметры командной строки для операций индексирования диспетчера области сканирования (CSM).
ms.assetid: 8c82fe18-8676-43d2-a3da-027a733ee0a4
title: кравлскопекоммандлине
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3eb770c44f82af320e2b39fe679b632cf03825e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572550"
---
# <a name="crawlscopecommandline"></a>кравлскопекоммандлине

В образце кода Кравлскопекоммандлине показано, как определить параметры командной строки для операций индексирования диспетчера области сканирования (CSM).

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

| Расположение | Путь или URL-адрес                                                                |
|----------|----------------------------------------------------------------------------|
| GitHub   |    [Пример Кравлскопекоммандлине](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/WindowsSearch/CrawlScopeCommandLine)|

> [!NOTE]  
> для всех версий Windows, включая Windows 7, рекомендуется загружать образцы непосредственно из GitHub для наиболее актуальной версии.

## <a name="building-the-sample"></a>Построение образца

1. откройте обозреватель Windows и перейдите в каталог проекта **кравлскопекоммандлине** .
2. Дважды щелкните значок файла ксмкмд. sln, чтобы открыть проект в Visual Studio.
  
    > [!NOTE]  
    > файл sln был создан в более ранней версии Visual Studio, поэтому его обновление потребуется при использовании Visual Studio 2012 или более поздних версий. Это не повлияет на поведение образца.

3. В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1. перейдите в каталог, содержащий новый исполняемый файл, используя окно командной строки или проводник Windows.
2. в командной строке введите `csmcmd.exe` или в Windows Explorer дважды щелкните значок csmcmd.exe.

## <a name="related-topics"></a>Связанные темы

### <a name="reference"></a>Справочник

[**иенумсеарчрутс**](/windows/desktop/api/Searchapi/nn-searchapi-ienumsearchroots)

[**иенумсеарчскоперулес**](/windows/desktop/api/Searchapi/nn-searchapi-ienumsearchscoperules)

[**исеарчкравлскопеманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcrawlscopemanager)

[**ISearchCrawlScopeManager2**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcrawlscopemanager2)

[**исеарчрут**](/windows/desktop/api/Searchapi/nn-searchapi-isearchroot)

[**исеарчскоперуле**](/windows/desktop/api/Searchapi/nn-searchapi-isearchscoperule)

[**исеарчкаталогманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager)

[**ISearchCatalogManager2**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager2)

[**исеарчманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchmanager)

### <a name="other-samples"></a>Другие примеры

[Поиск примеров кода](-search-samples-ovw.md)
