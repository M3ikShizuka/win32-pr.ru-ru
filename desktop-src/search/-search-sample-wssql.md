---
description: в примере кода всскл показано, как взаимодействовать между Microsoft OLE DB и Windows поиска с помощью язык SQL (SQL).
ms.assetid: 28663608-66b3-4404-9426-5a4b5f52a408
title: всскл
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5ac8f76b995d21a562f843344d1722cecec433af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363217"
---
# <a name="wssql"></a>всскл

в примере кода всскл показано, как взаимодействовать между Microsoft OLE DB и Windows поиска с помощью язык SQL (SQL).

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

| Расположение      | URL-адрес пути                                                                  |
|---------------|---------------------------------------------------------------------------|
| GitHub        | [Пример ВССКЛ](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/WindowsSearch/WSSQL)           |

> [!NOTE]  
> для всех версий Windows, включая Windows 7, рекомендуется загружать образцы непосредственно из GitHub для наиболее актуальной версии.

## <a name="building-the-sample"></a>Построение образца

1. откройте обозреватель Windows и перейдите в каталог проекта **всскл** .
2. Дважды щелкните значок файла ВССКЛ. sln, чтобы открыть проект в Visual Studio.
    > [!NOTE]  
    > файл sln был создан в более ранней версии Visual Studio, поэтому его обновление потребуется при использовании Visual Studio 2012 или более поздних версий. Это не повлияет на поведение образца.

3. В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1. перейдите в каталог, содержащий новый исполняемый файл, используя окно командной строки или проводник Windows.
2. в командной строке введите `WSSQL.exe` или в Windows Explorer дважды щелкните значок WSSQL.exe.

## <a name="related-topics"></a>Связанные темы

### <a name="conceptual"></a>Основные понятия

[использование синтаксиса SQL Windows Search](-search-sql-windowssearch-entry.md)

[Общие сведения о языке запросов](-search-sql-generalqueryinfo.md)

[Общие сведения о программировании OLE DB](/cpp/data/oledb/ole-db-programming-overview)

### <a name="other-samples"></a>Другие примеры

[Поиск примеров кода](-search-samples-ovw.md)
