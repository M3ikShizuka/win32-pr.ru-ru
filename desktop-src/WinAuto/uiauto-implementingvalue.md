---
title: Шаблон элемента управления Value
description: Описывает правила и соглашения для реализации Ивалуепровидер, включая сведения о свойствах и методах.
ms.assetid: 6b11d281-aca7-4548-853c-e7322999825d
keywords:
- Модель автоматизации пользовательского интерфейса, реализация шаблона элемента управления Value
- Модель автоматизации пользовательского интерфейса, шаблон элемента управления Value
- Модель автоматизации пользовательского интерфейса, Ивалуепровидер
- IValueProvider
- реализация шаблонов элементов управления "значение модели автоматизации пользовательского интерфейса"
- Шаблоны элементов управления Value
- шаблоны элементов управления, Ивалуепровидер
- шаблоны элементов управления, реализация значения автоматизации пользовательского интерфейса
- шаблоны элементов управления, значение
- интерфейсы, Ивалуепровидер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 40633a21fdd6b59a2aa35c34258037582a647f05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342763"
---
# <a name="value-control-pattern"></a>Шаблон элемента управления Value

Описывает правила и соглашения для реализации [**ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider), включая сведения о свойствах и методах. Шаблон элемента управления **value** используется для поддержки элементов управления с внутренним значением, не охватывающим диапазон, которые могут быть представлены в виде строки.

Строку значения можно изменять в зависимости от элемента управления и его параметров. Примеры элементов управления, реализующих этот шаблон элемента управления, см. в разделе [типы элементов управления и поддерживаемые шаблоны элементов управления](uiauto-controlpatternmapping.md).

В этом разделе содержатся следующие подразделы.

-   [Правила и соглашения реализации](#implementation-guidelines-and-conventions)
-   [Обязательные члены для **ивалуепровидер**](#required-members-for-ivalueprovider)
-   [Связанные темы](#related-topics)

## <a name="implementation-guidelines-and-conventions"></a>Правила и соглашения реализации

При реализации шаблона элемента управления **value** Обратите внимание на следующие правила и соглашения.

-   Элементы управления, такие как элемент списка или элемент дерева, должны поддерживать шаблон элемента управления **value** , если значение любого из элементов доступно для редактирования, независимо от текущего режима редактирования элемента управления. Родительский элемент управления также должен поддерживать шаблон элемента управления **value** , если дочерние элементы доступны для редактирования. На следующем рисунке показан пример изменяемого элемента списка.

    ![Иллюстрация, демонстрирующая редактируемый элемент списка](images/uia-valuepattern-editable-listitem.jpg)

- Одинарные и многострочные элементы управления редактирования должны реализовывать [**итекстпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) , чтобы предоставить доступ к содержимому только для чтения.
- Элементы управления для многострочного редактирования должны реализовывать [**ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider) , если их содержимое можно изменить.
- [**Ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider) не поддерживает извлечение сведений о форматировании или значений подстрок. Реализуйте [**итекстпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) в этих сценариях.
- [**ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider) должен быть реализован элементами управления, такими как элемент управления выбора цвета, из Microsoft Word (см. следующий рисунок), который поддерживает строковое сопоставление между значением цвета (например, "желтый") и эквивалентным внутренним значением [RGB](/windows/win32/api/wingdi/nf-wingdi-rgb) .

    ![Иллюстрация, показывающая сопоставление строк цветовой палитры](images/uia-valuepattern-colorpicker.jpg)

- Свойство "IsReadOnly" элемента управления должно иметь значение **true** , **а свойство** [**итекстпровидер:: IsReadOnly**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-get_isreadonly) — значение **false** , прежде чем разрешить вызов [**итекстпровидер:: SetValue**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-setvalue).

## <a name="required-members-for-ivalueprovider"></a>Обязательные члены для **ивалуепровидер**

Для реализации интерфейса [**ивалуепровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider) требуются следующие свойства и методы.



| Обязательные члены                                       | Тип члена | Примечания |
|--------------------------------------------------------|-------------|-------|
| [**IsReadOnly**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-get_isreadonly) | Свойство.    | None  |
| [**Значение**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-get_value)           | Свойство.    | None  |
| [**SetValue**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-ivalueprovider-setvalue)     | Метод      | None  |



 

Этот шаблон элемента управления не имеет связанных событий.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Типы элементов управления и поддерживаемые ими шаблоны элементов управления](uiauto-controlpatternmapping.md)
</dt> <dt>

[Общие сведения о шаблонах элементов управления модели автоматизации пользовательского интерфейса](uiauto-controlpatternsoverview.md)
</dt> <dt>

[Общие сведения о дереве модели автоматизации пользовательского интерфейса](uiauto-treeoverview.md)
</dt> <dt>

[Шаблоны элементов управления Text и TextRange](uiauto-implementingtextandtextrange.md)
</dt> </dl>

 

 