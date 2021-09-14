---
title: Элемент управления ToolTip (Справочник по элементам пользовательского интерфейса MSAA)
description: Элемент управления ToolTip отображает небольшое всплывающее окно, содержащее строку текста, описывающую Назначение инструмента, представленное в виде графического объекта в приложении.
ms.assetid: d3a65d7b-b882-4a1a-bac2-6995b64cf4af
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 37557fd116084fc9ac53e8567afc90eda339750d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064059"
---
# <a name="tooltip-control-msaa-ui-element-reference"></a>Элемент управления ToolTip (Справочник по элементам пользовательского интерфейса MSAA)

> [!Note]  
> В этом разделе описываются объекты **элементов управления ToolTip** для обращения к ЭЛЕМЕНТУ ПОЛЬЗОВАТЕЛЬСКОГО интерфейса MSAA. Создание объектов **элементов управления ToolTip** в различных ПЛАТФОРМАХ пользовательского интерфейса не описывается здесь. См. справочную документацию по API для платформы пользовательского интерфейса, которую вы используете.

 

Элемент управления ToolTip отображает небольшое всплывающее окно, содержащее строку текста, описывающую Назначение инструмента, представленное в виде графического объекта в приложении.

Имя класса Window для подсказки — это класс подсказок TOOLTIP \_ , который определен как "класс подсказок \_ " в коммктрл. h.

## <a name="iaccessible-methods"></a>Методы IAccessible

Элемент управления ToolTip поддерживает следующие методы [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :

-   [**акчиттест**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acchittest)
-   [**акклокатион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acclocation)
-   [**аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)
-   [**аккселект**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accselect)

## <a name="iaccessible-properties"></a>Свойства IAccessible

Элемент управления ToolTip поддерживает следующие свойства [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :



| Свойство.                                                                 | Комментарии                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**получить \_ аккчилдкаунт**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchildcount) | Свойство **ChildCount** равно нулю.                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [**получить \_ аккфокус**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accfocus)           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**получить \_ аккнаме**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname)             | Свойство **Name** — это текст, содержащийся в элементе управления ToolTip.                                                                                                                                                                                                                                                                                                                                                                                                       |
| [**получить \_ аккпарент**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent)         | **Родительское** свойство является окном ( [**\_ \_ окно системы ролей**](object-roles.md) ), которое окружает элемент управления и имеет **то же имя** свойства и класса окна, что и элемент управления.                                                                                                                                                                                                                                                               |
| [**получить \_ аккроле**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accrole)             | Свойство **Role** — [**\_ \_ Подсказка системы роли**](object-roles.md).                                                                                                                                                                                                                                                                                                                                                                               |
| [**получить \_ аккстате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accstate)           | Свойство **State** представляет собой сочетание одного или нескольких из следующих [значений](object-state-constants.md): [**\_ \_ невидимая**](object-state-constants.md) система состояния система состояния \| [**\_ \_ недоступна**](object-state-constants.md) система состояний, \| [**\_ \_ сфокусированная**](object-state-constants.md) на \| [**\_ \_ системе состояния**](object-state-constants.md)<br/> |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Интерфейс IAccessible](/windows/desktop/api/oleacc/nn-oleacc-iaccessible)
</dt> </dl>

 

 





