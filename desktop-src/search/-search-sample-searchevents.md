---
description: В образце кода Сеарчевентс показано, как задать приоритет событий индексирования.
ms.assetid: a352c3e2-5860-4b9c-a3c7-a806f69b4f7d
title: сеарчевентс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 21472d113694a41a3c7855c0fdaf8f2fa2b3b2e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363233"
---
# <a name="searchevents"></a>сеарчевентс

В образце кода Сеарчевентс показано, как задать приоритет событий индексирования.

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
| GitHub        | [Пример Сеарчевентс](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/WindowsSearch/SearchEvents)    |

> [!NOTE]  
> для всех версий Windows, включая Windows 7, рекомендуется загружать образцы непосредственно из GitHub для наиболее актуальной версии.

## <a name="building-the-sample"></a>Построение образца

1. откройте обозреватель Windows и перейдите в каталог проекта **сеарчевентс** .
2. Дважды щелкните значок файла Eventing. sln, чтобы открыть проект в Visual Studio.
  
    > [!NOTE]  
    > файл sln был создан в более ранней версии Visual Studio, поэтому его обновление потребуется при использовании Visual Studio 2012 или более поздних версий. Это не повлияет на поведение образца.

3. В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1. перейдите в каталог, содержащий новый исполняемый файл, используя окно командной строки или проводник Windows.
2. в командной строке введите `Eventing.exe` или в Windows Explorer дважды щелкните значок Eventing.exe.

## <a name="related-topics"></a>Связанные темы

### <a name="reference"></a>Справочник

[**ировсетевентс**](/windows/desktop/api/Searchapi/nn-searchapi-irowsetevents)

[**ировсетприоритизатион**](/windows/desktop/api/Searchapi/nn-searchapi-irowsetprioritization)

[**уровень ПРИОРИТЕТа \_**](/windows/win32/api/searchapi/ne-searchapi-priority_level)

[**РОВСЕТЕВЕНТ \_ ITEMSTATE**](/windows/win32/api/searchapi/ne-searchapi-rowsetevent_itemstate)

[**\_тип ровсетевент**](/windows/win32/api/searchapi/ne-searchapi-rowsetevent_type)

### <a name="other-samples"></a>Другие примеры

[Поиск примеров кода](-search-samples-ovw.md)
