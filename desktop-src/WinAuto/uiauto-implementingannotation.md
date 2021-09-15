---
title: Шаблон элемента Annotation
description: Описывает правила и соглашения для реализации Ианнотатионпровидер, включая сведения о свойствах и методах. Шаблон элемента управления Annotation используется для предоставления свойств заметки в документе.
ms.assetid: 5A334991-66AF-4A82-9A09-09D5BDAAA771
keywords:
- Модель автоматизации пользовательского интерфейса, реализация шаблона элемента управления Annotation
- Модель автоматизации пользовательского интерфейса, шаблон элемента управления Annotation
- Модель автоматизации пользовательского интерфейса, Ианнотатионпровидер
- IAnnotationProvider
- Реализация шаблона элемента управления заметки модели автоматизации пользовательского интерфейса
- шаблон элемента Annotation
- шаблоны элементов управления, Ианнотатионпровидер
- шаблоны элементов управления, реализация аннотации автоматизации пользовательского интерфейса
- шаблоны элементов управления, аннотация
- интерфейсы, Ианнотатионпровидер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1c1a0441816e548faaa9076b3a9717c0aa76f08a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567254"
---
# <a name="annotation-control-pattern"></a>Шаблон элемента Annotation

Описывает правила и соглашения для реализации [**ианнотатионпровидер**](/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider), включая сведения о свойствах и методах. Шаблон элемента управления **Annotation** используется для предоставления свойств заметки в документе.

Одним из примеров является всплывающая подсказка с комментарием, расположенная на поле документа и подключенная к тексту документа или ячейке таблицы.

На следующем рисунке показан пример заметки. Примеры элементов управления, реализующих этот шаблон элемента управления, см. в разделе [типы элементов управления и поддерживаемые шаблоны элементов управления](uiauto-controlpatternmapping.md).

![снимок экрана с комментарием, балун в документе](images/annotation.png)

В этом разделе содержатся следующие подразделы.

-   [Правила и соглашения реализации](#implementation-guidelines-and-conventions)
-   [Обязательные члены для **ианнотатионпровидер**](#required-members-for-iannotationprovider)
-   [Связанные разделы](#related-topics)

## <a name="implementation-guidelines-and-conventions"></a>Правила и соглашения реализации

При реализации шаблона элемента управления **Annotation** Обратите внимание на следующие правила и соглашения.

-   Существует много различных типов заметок. Файл заголовка UIAutomationClient. h определяет набор именованных постоянных значений, которые определяют типы заметок, поддерживаемых Microsoft UI Automation. Дополнительные сведения см. в разделе [**идентификаторы типов заметок**](uiauto-annotation-type-identifiers.md).
-   Если используется [**аннотатионтипе \_ Unknown**](uiauto-annotation-type-identifiers.md), необходимо реализовать свойство [**ианнотатионпровидер:: аннотатионтипенаме**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_annotationtypename) , чтобы позволить клиентам обнаруживать имя типа заметки. Не нужно реализовывать **аннотатионтипенаме** для стандартного типа заметки, так как модель автоматизации пользовательского интерфейса предоставляет имя по умолчанию, но его можно реализовать, если необходимо переопределить имя по умолчанию.
-   Свойство [**ианнотатионпровидер:: Author**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_author) является необязательным.
-   Свойство [**ианнотатионпровидер::D атетиме**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_datetime) является необязательным.
-   Свойство [**ианнотатионпровидер:: target**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_target) является обязательным, так как оно связывает заметку с элементом пользовательского интерфейса, позволяя клиенту переходить от заметки к ЭЛЕМЕНТУ пользовательского интерфейса, к которому относится Аннотация.
-   Поскольку заметки могут принимать множество различных форм, интерфейс [**ианнотатионпровидер**](/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider) не определяет свойство для хранения значения или текста заметки. Простая Аннотация должна предоставлять доступ к интерфейсу [**ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider) , а свойство [**Ивалуепровидер:: value**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-get_value) должно возвращать значение только для чтения, указывающее текст заметки. Более широкая Аннотация должна предоставлять интерфейс [**итекстпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) для предоставления клиентам более обширного текста.
-   Переход от элемента пользовательского интерфейса к заметке в элементе зависит от вида элемента, для которого записываются аннотации, следующим образом:
    -   Для ячеек таблицы реализуйте метод [**испреадшититемпровидер:: жетаннотатионобжектс**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-ispreadsheetitemprovider-getannotationobjects) для ссылки на заметку.
    -   Для текстового содержимого реализуйте атрибут Text [**аннотатионобжектс**](uiauto-textattribute-ids.md) в интерфейсе [**итекстранжепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextrangeprovider) для ссылки на заметку.
-   Некоторые типы заметок не нуждаются в полной реализации интерфейса [**ианнотатионпровидер**](/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider) . Например, можно представить простой индикатор орфографической ошибки, если интерфейс [**итекстранжепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextrangeprovider) возвращает атрибут [**аннотатионтипес**](uiauto-textattribute-ids.md) Text [**аннотатионтипе \_ Спеллинжеррор**](uiauto-annotation-type-identifiers.md)и значение NULL для атрибута [**аннотатионобжектс**](uiauto-textattribute-ids.md) Text.
-   Может быть полезно реализовать интерфейс [**ианнотатионпровидер**](/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider) в невидимом ЭЛЕМЕНТЕ пользовательского интерфейса. Например, можно создать невидимый элемент автоматизации пользовательского интерфейса, реализующий **ианнотатионпровидер** для предоставления расширенной информации об грамматической ошибке.
-   Аннотации в элементе управления на основе текста могут быть сложными, если элемент управления содержит перекрывающиеся комментарии. Используйте следующие рекомендации для работы с сложными заметками:
    -   Текстовый диапазон без заметок должен возвращать пустой массив для текстового атрибута [**аннотатионтипес**](uiauto-textattribute-ids.md) и пустой массив для атрибута Text [**аннотатионобжектс**](uiauto-textattribute-ids.md) .
    -   Текстовый диапазон с одной заметкой должен возвращать массив из одного целочисленного значения для текстового атрибута [**аннотатионтипес**](uiauto-textattribute-ids.md) и массив из одного интерфейса [**иравелементпровидерсимпле**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-irawelementprovidersimple) для текстового атрибута [**аннотатионобжектс**](uiauto-textattribute-ids.md) .
    -   Текстовый диапазон с несколькими заметками должен возвращать массив из нескольких целочисленных значений для атрибута Text [**аннотатионтипес**](uiauto-textattribute-ids.md) и массив соответствующего числа интерфейсов [**иравелементпровидерсимпле**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-irawelementprovidersimple) для атрибута Text [**аннотатионобжектс**](uiauto-textattribute-ids.md) .
    -   Текстовый диапазон с различными заметками, например диапазон с заметками и текстом без заметок, должен возвращать свойство [**ресерведмикседаттрибутевалуе**](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-uiagetreservedmixedattributevalue) для [**аннотатионтипес**](uiauto-textattribute-ids.md) и [**аннотатионобжектс**](uiauto-textattribute-ids.md). Клиент, получивший этот ответ, может разделить текстовый диапазон, чтобы найти место начала и конца заметок.

## <a name="required-members-for-iannotationprovider"></a>Обязательные члены для **ианнотатионпровидер**

Для реализации интерфейса [**ианнотатионпровидер**](/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider) требуются следующие свойства.



| Обязательные члены                                                                | Тип члена | Примечания |
|---------------------------------------------------------------------------------|-------------|-------|
| [**аннотатионтипеид**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_annotationtypeid)     | Свойство    | Нет. |
| [**аннотатионтипенаме**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_annotationtypename) | Свойство    | Нет. |
| [**Автор**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_author)                         | Свойство    | Нет. |
| [**DateTime**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_datetime)                     | Свойство    | Нет. |
| [**Мишень**](/windows/desktop/api/uiautomationcore/nf-uiautomationcore-iannotationprovider-get_target)                         | Свойство    | Нет. |



 

Этот шаблон элемента управления не имеет связанных событий.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Типы элементов управления и поддерживаемые ими шаблоны элементов управления](uiauto-controlpatternmapping.md)
</dt> <dt>

[Общие сведения о шаблонах элементов управления модели автоматизации пользовательского интерфейса](uiauto-controlpatternsoverview.md)
</dt> <dt>

[Общие сведения о дереве модели автоматизации пользовательского интерфейса](uiauto-treeoverview.md)
</dt> </dl>

 

 