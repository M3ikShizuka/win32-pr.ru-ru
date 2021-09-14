---
title: Шаблон элемента управления Мултиплевиев
description: Описывает правила и соглашения для реализации IMultipleViewProvider, включая сведения о свойствах и методах.
ms.assetid: c67e7e4f-d2c7-4fca-8e8a-9b6565afa4ed
keywords:
- Модель автоматизации пользовательского интерфейса, реализация шаблона элемента управления Мултиплевиев
- Модель автоматизации пользовательского интерфейса, шаблон элемента управления Мултиплевиев
- Модель автоматизации пользовательского интерфейса, IMultipleViewProvider
- IMultipleViewProvider
- реализация шаблонов элементов управления Мултиплевиев модели автоматизации пользовательского интерфейса
- Шаблоны элементов управления Мултиплевиев
- шаблоны элементов управления, IMultipleViewProvider
- шаблоны элементов управления, реализация модели автоматизации пользовательского интерфейса Мултиплевиев
- шаблоны элементов управления, Мултиплевиев
- интерфейсы, IMultipleViewProvider
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d4bc5d1991e99f1338853aac528111d8ec3ca3c2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058448"
---
# <a name="multipleview-control-pattern"></a>Шаблон элемента управления Мултиплевиев

Описывает правила и соглашения для реализации [**IMultipleViewProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-imultipleviewprovider), включая сведения о свойствах и методах. Ссылки на дополнительные материалы перечислены в конце раздела. Шаблон элемента управления **мултиплевиев** используется для поддержки элементов управления, которые предоставляют и могут переключаться между несколькими представлениями одних и тех же сведений или одного набора дочерних элементов управления.

примеры элементов управления, которые могут представлять несколько представлений, включают представление списка (которое может отображать его содержимое в виде эскизов, плитки, значки или сведения), Microsoft Excel диаграммы (круговые, линейные, линейчатые, значения ячеек с формулой), Microsoft Word документы (обычные, веб-макет, макет печати, макет для чтения, контур), календарь microsoft Outlook (год, месяц, неделя, день) и обложки microsoft проигрыватель Windows Media. Поддерживаемые представления определяются разработчиками элементов управления и относятся к конкретному элементу управления.

В этом разделе содержатся следующие подразделы.

-   [Правила и соглашения реализации](#implementation-guidelines-and-conventions)
-   [Обязательные члены для **IMultipleViewProvider**](#required-members-for-imultipleviewprovider)
-   [Связанные темы](#related-topics)

## <a name="implementation-guidelines-and-conventions"></a>Правила и соглашения реализации

При реализации шаблона элемента управления **мултиплевиев** Обратите внимание на следующие правила и соглашения.

-   [**IMultipleViewProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-imultipleviewprovider) также должен быть реализован в контейнере, который управляет текущим представлением, если он отличается от элемента управления, предоставляющего текущее представление. например, Windows explorer содержит элемент управления "список" для текущего содержимого папки, в то время как представление элемента управления управляется из приложения "обозреватель Windows".
-   Элемент управления, который может сортировать свое содержимое, не считается поддерживающим несколько представлений.
-   Коллекция представлений должна быть идентичной во всех экземплярах.
-   Имена представлений должны быть подходящими для использования в тексте для распознавания речи, шрифта Брайля и других приложений, пригодных для восприятия.

## <a name="required-members-for-imultipleviewprovider"></a>Обязательные члены для **IMultipleViewProvider**

Для реализации интерфейса [**IMultipleViewProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-imultipleviewprovider) требуются следующие свойства и методы.



| Обязательные члены                                                            | Тип члена | Примечания |
|-----------------------------------------------------------------------------|-------------|-------|
| [**куррентвиев**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-imultipleviewprovider-get_currentview)             | Свойство.    | Нет  |
| [**жетсуппортедвиевс**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-imultipleviewprovider-getsupportedviews) | Метод      | None  |
| [**жетвиевнаме**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-imultipleviewprovider-getviewname)             | Метод      | None  |
| [**сеткуррентвиев**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-imultipleviewprovider-setcurrentview)       | Метод      | None  |



 

Этот шаблон элемента управления не имеет связанных событий.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Типы элементов управления и поддерживаемые ими шаблоны элементов управления](uiauto-controlpatternmapping.md)
</dt> <dt>

[Общие сведения о шаблонах элементов управления модели автоматизации пользовательского интерфейса](uiauto-controlpatternsoverview.md)
</dt> <dt>

[Общие сведения о дереве модели автоматизации пользовательского интерфейса](uiauto-treeoverview.md)
</dt> <dt>

[Шаблон элемента управления ExpandCollapse](uiauto-implementingexpandcollapse.md)
</dt> </dl>

 

 




