---
title: Шаблон элемента управления Window
description: Описывает правила и соглашения для реализации IWindowProvider, включая сведения о свойствах, методах и событиях. Шаблон элемента управления Window поддерживает элементы управления, обеспечивающие фундаментальные функции на основе окна в традиционном графическом интерфейсе пользователя.
ms.assetid: bfd37d27-fcec-4d25-841c-63e14e48c6c8
keywords:
- Модель автоматизации пользовательского интерфейса, реализация шаблона элемента управления Window
- Модель автоматизации пользовательского интерфейса, шаблон элемента управления Window
- Модель автоматизации пользовательского интерфейса, IWindowProvider
- IWindowProvider
- реализация шаблонов элементов управления окна модели автоматизации пользовательского интерфейса
- Шаблоны элементов управления Window
- шаблоны элементов управления, IWindowProvider
- шаблоны элементов управления, реализация окна модели автоматизации пользовательского интерфейса
- шаблоны элементов управления, окно
- интерфейсы, IWindowProvider
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b3c4f0d862a14fee35f8d1982c7870e2be031c61
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242362"
---
# <a name="window-control-pattern"></a>Шаблон элемента управления Window

Описывает правила и соглашения для реализации [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider), включая сведения о свойствах, методах и событиях. Шаблон элемента управления **Window** поддерживает элементы управления, обеспечивающие фундаментальные функции на основе окна в традиционном графическом интерфейсе пользователя.

Примеры элементов управления, которые должны реализовывать этот шаблон элемента управления, включают в себя окна приложений верхнего уровня, дочерние окна многодокументного интерфейса (MDI), элементы управления "область разделения" с изменяемыми размерами, модальные диалоговые окна и окна справки. Примеры элементов управления, реализующих данный шаблон элемента управления, см. в разделе [Control Pattern Mapping for UI Automation Clients](uiauto-controlpatternmapping.md).

В этом разделе содержатся следующие подразделы.

-   [Правила и соглашения реализации](#implementation-guidelines-and-conventions)
-   [Обязательные члены для **IWindowProvider**](#required-members-for-iwindowprovider)
-   [Связанные темы](#related-topics)

## <a name="implementation-guidelines-and-conventions"></a>Правила и соглашения реализации

При реализации шаблона элемента управления **Window** Обратите внимание на следующие правила и соглашения.

-   Чтобы обеспечить возможность изменения размера окна и расположения экрана с помощью автоматизации пользовательского интерфейса Майкрософт, элемент управления должен реализовать [**итрансформпровидер**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itransformprovider) в дополнение к [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider).
-   Элементы управления, содержащие заголовки заголовков и элементы заголовка, позволяющие перемещать элемент управления, изменять его размер, разворачивание, свернутый или закрываемый, обычно необходимы для реализации [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider).
-   Элементы управления, такие как всплывающие подсказки и поля со списком или раскрывающиеся меню, обычно не реализуют [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider).
-   Всплывающие окна справки изменяются от отображения окон основных всплывающих подсказок за счет предоставления кнопки **закрытия** , подобной окну.
-   Полноэкранный режим не поддерживается [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider) , так как он относится к конкретному приложению и не является обычным поведением окна.

## <a name="required-members-for-iwindowprovider"></a>Обязательные члены для **IWindowProvider**

Для реализации интерфейса [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider) требуются следующие свойства, методы и события.



| Обязательные члены                                                                            | Тип члена | Примечания                                                                       |
|---------------------------------------------------------------------------------------------|-------------|-----------------------------------------------------------------------------|
| [**виндовинтерактионстате**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_windowinteractionstate)             | Свойство.    | Не гарантируется, что **виндовинтерактионстате \_ реадифорусеринтерактион** |
| [**Modal**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_ismodal)                                           | Свойство.    | None                                                                        |
| [**По верхнему уровню**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_istopmost)                                       | Свойство.    | None                                                                        |
| [**канмаксимизе**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_canmaximize)                                   | Свойство.    | None                                                                        |
| [**канминимизе**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_canminimize)                                   | Свойство.    | None                                                                        |
| [**виндоввисуалстате**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-get_windowvisualstate)                       | Свойство.    | None                                                                        |
| [**Выхода**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-close)                                               | Метод      | None                                                                        |
| [**сетвисуалстате**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-setvisualstate)                             | Метод      | None                                                                        |
| [**ваитфоринпутидле**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-iwindowprovider-waitforinputidle)                         | Метод      | None                                                                        |
| [**\_Окно UIA \_ виндовклоседевентид**](uiauto-event-ids.md) | Событие       | None                                                                        |
| [**\_Окно UIA \_ виндовопенедевентид**](uiauto-event-ids.md) | Событие       | None                                                                        |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Общие сведения о шаблонах элементов управления модели автоматизации пользовательского интерфейса](uiauto-controlpatternsoverview.md)
</dt> <dt>

[Сопоставление шаблона элемента управления для клиентов автоматизации пользовательского интерфейса](uiauto-controlpatternmapping.md)
</dt> <dt>

[Общие сведения о дереве модели автоматизации пользовательского интерфейса](uiauto-treeoverview.md)
</dt> </dl>

 

 




