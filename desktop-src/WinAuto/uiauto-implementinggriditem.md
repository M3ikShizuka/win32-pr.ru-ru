---
title: Шаблон элемента управления GridItem
description: Описывает правила и соглашения для реализации Игридитемпровидер, включая сведения о свойствах. Шаблон элемента управления GridItem используется для поддержки отдельных дочерних элементов управления контейнеров, реализующих IGridProvider.
ms.assetid: ae4b9021-1800-485b-99a2-54ddf9c21f93
keywords:
- Модель автоматизации пользовательского интерфейса, реализация шаблона элемента управления GridItem
- Модель автоматизации пользовательского интерфейса, шаблон элемента управления GridItem
- Модель автоматизации пользовательского интерфейса, Игридитемпровидер
- IGridItemProvider
- реализация шаблонов элементов управления GridItem модели автоматизации пользовательского интерфейса
- Шаблоны элементов управления GridItem
- шаблоны элементов управления, Игридитемпровидер
- шаблоны элементов управления, реализация GridItem в модели автоматизации пользовательского интерфейса
- шаблоны элементов управления, GridItem
- интерфейсы, Игридитемпровидер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2ef45b5f655e3ef09350c508271233de49f964a4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058459"
---
# <a name="griditem-control-pattern"></a>Шаблон элемента управления GridItem

Описывает правила и соглашения для реализации [**игридитемпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igriditemprovider), включая сведения о свойствах. Шаблон элемента управления **GridItem** используется для поддержки отдельных дочерних элементов управления контейнеров, реализующих [**IGridProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igridprovider).

Примеры элементов управления, реализующих этот шаблон элемента управления, см. в разделе [типы элементов управления и поддерживаемые шаблоны элементов управления](uiauto-controlpatternmapping.md).

В этом разделе содержатся следующие подразделы.

-   [Правила и соглашения реализации](#implementation-guidelines-and-conventions)
-   [Обязательные члены для **игридитемпровидер**](#required-members-for-igriditemprovider)
-   [Связанные темы](#related-topics)

## <a name="implementation-guidelines-and-conventions"></a>Правила и соглашения реализации

При реализации шаблона элемента управления **GridItem** Обратите внимание на следующие правила и соглашения.

-   Координаты сетки отсчитываются от нуля, начиная с верхней левой ячейки с координатами (0, 0).
-   Объединенные ячейки будут сообщать о свойствах [**строк**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_row) и [**столбцов**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_column) в зависимости от базовой ячейки привязки, как определено поставщиком автоматизации пользовательского интерфейса Майкрософт. Как правило, это будет самая верхняя строка и крайний левый столбец.
-   [**IGridProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igridprovider) не обеспечивает активную обработку сетки, например объединение или разбиение ячеек.
-   Элементы управления, которые реализуют [**IGridProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igridprovider) , обычно обходятся (то есть клиент автоматизации пользовательского интерфейса могут переходить к смежным элементам управления) с помощью клавиатуры.

## <a name="required-members-for-igriditemprovider"></a>Обязательные члены для **игридитемпровидер**

Для реализации интерфейса [**игридитемпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igriditemprovider) требуются следующие свойства.



| Обязательные члены                                                  | Тип члена | Примечания |
|-------------------------------------------------------------------|-------------|-------|
| [**Строки**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_row)                       | Свойство.    | None  |
| [**Рубрик**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_column)                 | Свойство.    | Нет  |
| [**RowSpan**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_rowspan)               | Свойство.    | None  |
| [**ColumnSpan**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_columnspan)         | Свойство.    | Нет  |
| [**контаининггрид**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-igriditemprovider-get_containinggrid) | Свойство.    | Нет  |



 

Этот шаблон элемента управления не имеет связанных методов или событий.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Типы элементов управления и поддерживаемые ими шаблоны элементов управления](uiauto-controlpatternmapping.md)
</dt> <dt>

[Шаблон элемента управления Grid](uiauto-implementinggrid.md)
</dt> <dt>

[Общие сведения о шаблонах элементов управления модели автоматизации пользовательского интерфейса](uiauto-controlpatternsoverview.md)
</dt> <dt>

[Общие сведения о дереве модели автоматизации пользовательского интерфейса](uiauto-treeoverview.md)
</dt> </dl>

 

 




