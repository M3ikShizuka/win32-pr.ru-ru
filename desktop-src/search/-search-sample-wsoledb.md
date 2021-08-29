---
description: в примере кода всоледб демонстрируется использование библиотеки atl OLE DB доступ к приложениям поиска Windows, а также демонстрируются два дополнительных метода получения результатов поиска Windows.
ms.assetid: c81bf3af-e023-4384-8c89-0fa9c8f08773
title: всоледб
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 17000de683fc9f5171bc556c607c7c068cabb4b3e88693407e1381565fb6b242
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118969623"
---
# <a name="wsoledb"></a>всоледб

в примере кода всоледб демонстрируется использование библиотеки atl OLE DB доступ к приложениям поиска Windows, а также демонстрируются два дополнительных метода получения результатов поиска Windows.

В этом разделе содержатся следующие подразделы.

- [Требования](#requirements)
- [Загрузка образца](#downloading-the-sample)
- [Создание примера](#building-the-sample)
- [Запуск примера](#running-the-sample)
- [Связанные темы](#related-topics)

## <a name="requirements"></a>Requirements (Требования)

| Продукт     | Версия продукта          |
|-------------|--------------------------|
| Windows     | Windows 7, 8.1 или 10    |
| Пакет Windows SDK | 7,0 или выше           |

## <a name="downloading-the-sample"></a>Загрузка образца

Этот пример доступен в следующем расположении.

| Расположение      | URL-адрес пути                                                                  |
|---------------|---------------------------------------------------------------------------|
| GitHub        | [Пример Всоледб](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/WindowsSearch/WSOleDB)         |

> [!NOTE]  
> для всех версий Windows, включая Windows 7, рекомендуется загружать образцы непосредственно из GitHub для наиболее актуальной версии.

## <a name="building-the-sample"></a>Построение образца

1. откройте обозреватель Windows и перейдите в каталог проекта **всоледб** .
2. Дважды щелкните значок файла Всоледб. sln, чтобы открыть проект в Visual Studio.
  
    > [!NOTE]  
    > файл sln был создан в более ранней версии Visual Studio, поэтому его обновление потребуется при использовании Visual Studio 2012 или более поздних версий. Это не повлияет на поведение образца.

3. В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1. перейдите в каталог, содержащий новый исполняемый файл, используя окно командной строки или проводник Windows.
2. в командной строке введите `WSOleDB.exe` или в Windows Explorer дважды щелкните значок WSOleDB.exe.

## <a name="related-topics"></a>Связанные темы

### <a name="reference"></a>Справочник

[**исеарчкаталогманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager)

[**ISearchCatalogManager2**](/windows/desktop/api/Searchapi/nn-searchapi-isearchcatalogmanager2)

[**исеарчманажер**](/windows/desktop/api/Searchapi/nn-searchapi-isearchmanager)

[**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore)

### <a name="conceptual"></a>Основные понятия

[Общие сведения о программировании OLE DB](/cpp/data/oledb/ole-db-programming-overview)

### <a name="other-samples"></a>Другие примеры

[Поиск примеров кода](-search-samples-ovw.md)
