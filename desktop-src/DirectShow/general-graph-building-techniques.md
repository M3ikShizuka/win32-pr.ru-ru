---
description: Общие методы Graph-Building
ms.assetid: 66d93305-175c-4549-b825-2f3d7fd6bf09
title: Общие методы Graph-Building
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 73c73a005f1fbf7af0a53f11d44d600852f88752
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053407"
---
# <a name="general-graph-building-techniques"></a>Общие методы Graph-Building

каждое DirectShow приложение начинается с создания графа фильтра. по мере ознакомления с обзорными разделами в документации по DirectShow вы обнаружите, что лучше всего начать с описания того, какой именно граф фильтра вам нужен. В некоторых случаях существует метод или вспомогательный объект, специально предназначенный для создания такого типа графа. например, объект [dvd Graph Builder](dvd-graph-builder.md) создает графы воспроизведения dvd-дисков. В других случаях приложение должно создать граф, добавив фильтры и соединив их.

В этом разделе представлены некоторые вспомогательные функции, реализующие базовые операции построения графа. они могут использоваться любым приложением DirectShow, которое должно создавать или изменять граф фильтра. В этом разделе рассматриваются следующие вопросы.

-   [Добавление фильтра по CLSID](add-a-filter-by-clsid.md)
-   [Поиск неподключенного ПИН-кода в фильтре](find-an-unconnected-pin-on-a-filter.md)
-   [Подключение Два фильтра](connect-two-filters.md)
-   [Поиск интерфейса в фильтре или ПИН-коде](find-an-interface-on-a-filter-or-pin.md)
-   [Поиск однорангового узла фильтра](find-a-filters-peer.md)
-   [Удалите все фильтры в Graph](remove-all-the-filters-in-the-graph.md)
-   [построение диаграмм с помощью построителя Graph Capture](building-graphs-with-the-capture-graph-builder.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[основные задачи DirectShow](basic-directshow-tasks.md)
</dt> <dt>

[Перечисление устройств и фильтров](enumerating-devices-and-filters.md)
</dt> <dt>

[Перечисление объектов в фильтре Graph](enumerating-objects-in-a-filter-graph.md)
</dt> <dt>

[интеллектуальные Подключение](intelligent-connect.md)
</dt> </dl>

 

 



