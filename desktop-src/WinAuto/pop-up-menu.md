---
title: Всплывающее меню (Справочник по элементам пользовательского интерфейса MSAA)
description: Во всплывающем меню отображается список команд меню.
ms.assetid: 9dbfa2d7-a086-4348-8b84-7e36d33e2d27
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 785fe8ac7a70352116b3a77cf30034092de04a23
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064127"
---
# <a name="pop-up-menu-msaa-ui-element-reference"></a>Всплывающее меню (Справочник по элементам пользовательского интерфейса MSAA)

> [!Note]  
> В этом разделе описываются объекты **всплывающего меню** в справочнике по элементам ПОЛЬЗОВАТЕЛЬСКОГО интерфейса MSAA. Создание объектов **всплывающего меню** в различных ПЛАТФОРМАХ пользовательского интерфейса не описывается здесь. См. справочную документацию по API для платформы пользовательского интерфейса, которую вы используете.

 

Во всплывающем меню отображается список команд меню. Microsoft Active Accessibility создает всплывающий объект меню при открытии пункта меню в строке меню. Кроме того, Microsoft Active Accessibility создает всплывающие меню для контекстных меню, которые отображаются, когда пользователь щелкает правой кнопкой мыши элемент пользовательского интерфейса.

Имя класса окон для всплывающего меню — " \# 32768".

## <a name="iaccessible-methods"></a>Методы IAccessible

Всплывающее меню поддерживает следующие методы [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :

-   [**акчиттест**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acchittest)
-   [**акклокатион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acclocation)
-   [**аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)
-   [**аккселект**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accselect)

## <a name="iaccessible-properties"></a>Свойства IAccessible

Всплывающее меню поддерживает следующие свойства [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :



| Свойство.                                                                 | Комментарии                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**получить \_ аккчилд**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchild)           | Извлекает [**IDispatch**](idispatch-interface.md) для указанного элемента меню. Идентификаторы дочерних элементов меню нумеруются последовательно сверху вниз, начиная с единицы.                                                                                                                                                                                                                                                                                      |
| [**получить \_ аккчилдкаунт**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchildcount) | Свойство **ChildCount** — это число пунктов меню в меню, включая разделители меню.                                                                                                                                                                                                                                                                                                                                                                           |
| [**получить \_ аккфокус**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accfocus)           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**получить \_ аккнаме**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname)             | Свойство **имя** всплывающего меню совпадает с именем меню. Свойство **Name** контекстного меню — «context».                                                                                                                                                                                                                                                                                                                                              |
| [**получить \_ аккпарент**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent)         | **Родительское** свойство является окном ( [**\_ \_ окно системы ролей**](object-roles.md) ), которое окружает всплывающее меню и имеет **то же имя** свойства и класса окна, что и всплывающее меню.                                                                                                                                                                                                                                                      |
| [**получить \_ аккроле**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accrole)             | Свойство **Role** имеет [**роль \_ System \_ менупопуп**](object-roles.md).                                                                                                                                                                                                                                                                                                                                                                           |
| [**получить \_ аккстате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accstate)           | Свойство **State** представляет собой сочетание одного или нескольких из следующих [значений](object-state-constants.md): [**\_ \_ невидимая**](object-state-constants.md) система состояния система состояния \| [**\_ \_ недоступна**](object-state-constants.md) система состояний, \| [**\_ \_ сфокусированная**](object-state-constants.md) на \| [**\_ \_ системе состояния**](object-state-constants.md)<br/> |



 

## <a name="notes"></a>Примечания

-   Объекты всплывающего меню не активируют события [**\_ \_ создания объектов событий**](event-constants.md) и [**\_ \_ уничтожения объектов событий**](event-constants.md) .
-   Меню с несколькими столбцами не поддерживают флаги [**навдир \_ Left**](navigation-constants.md) или [**навдир \_ right**](navigation-constants.md) метода [**аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate) .
-   Системные события и системные [**\_ \_ менупопупенд**](event-constants.md) событий событий [**\_ \_ менупопупстарт**](event-constants.md) не отправляются постоянно. Это известная проблема, которая решена.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Интерфейс IAccessible](/windows/desktop/api/oleacc/nn-oleacc-iaccessible)
</dt> <dt>

[**Строка меню**](menu-bar.md)
</dt> <dt>

[**Menu Item**](menu-item.md)
</dt> </dl>

 

 





