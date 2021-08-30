---
title: Заголовок окна (Справочник по элементу пользовательского интерфейса MSAA)
description: В строке заголовка в верхней части окна отображается значок и строка текста, определенные в приложении.
ms.assetid: f41ab777-6c94-4d8e-b743-c635e93df396
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 620fa8716cb498857cdf12c652b99f409e6e4214
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122480130"
---
# <a name="title-bar-msaa-ui-element-reference"></a>Заголовок окна (Справочник по элементу пользовательского интерфейса MSAA)

> [!Note]  
> В этом разделе описываются объекты **заголовков** для целей справочника по элементам ПОЛЬЗОВАТЕЛЬСКОГО интерфейса MSAA. Создание объектов **заголовка** в различных ПЛАТФОРМАХ пользовательского интерфейса не описывается здесь. См. справочную документацию по API для платформы пользовательского интерфейса, которую вы используете.

 

В строке заголовка в верхней части окна отображается значок и строка текста, определенные в приложении. Текст указывает имя приложения и указывает назначение окна. Кроме того, строка заголовка позволяет пользователю перемещать окно с помощью мыши или другого указывающего устройства.

Строки заголовка содержат по крайней мере три небольшие кнопки, которые сворачиваются, развернут или восстановлены, и закрывают окно, связанное с заголовком. Строки заголовка также содержат контекстно-зависимую кнопку справки. приложения, работающие в Far-East версии операционной системы Windows, также могут содержать кнопки редактора методов ввода (IME). Microsoft Active Accessibility предоставляет эти кнопки как дочерние элементы заголовка окна.

## <a name="iaccessible-methods"></a>Методы IAccessible

Строки заголовка поддерживают следующие методы [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :

-   [**акчиттест**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acchittest)
-   [**акклокатион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acclocation)
-   [**аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)
-   [**аккселект**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accselect)

## <a name="iaccessible-properties"></a>Свойства IAccessible

Заголовки окон поддерживают следующие свойства [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :




| Свойство | Комментарии | 
|----------|----------|
| <a href="/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchildcount"><strong>get_accChildCount</strong></a> | Свойство <strong>ChildCount</strong> имеет значение 5. Свойство <strong>ChildCount</strong> содержит редакторы IME и контекстно-зависимые кнопки справки, даже если они не отображаются. Кнопки, которые не отображаются, имеют <strong></strong> свойство State <a href="object-state-constants.md"><strong>STATE_SYSTEM_INVISIBLE</strong></a>. | 
| <strong>get_accDescription</strong> | Свойство <strong>Description</strong> в строке заголовка имеет значение: "отображает имя окна и содержит элементы управления для управления им". Дочерние кнопки в заголовке окна имеют следующие описания:<br /><ul><li>"Перемещает окно из</li><li>«Делает окно заполненным</li><li>"Помещает в сворачивания или</li><li>"Закрывает окно"</li><li>"Вводит или оставляет контекст-</li><li>"Открывает клавиатуру при нажатии"</li></ul> | 
| <strong>get_accName</strong> | Сама строка заголовка не поддерживает свойство <strong>Name</strong> . Дочерние кнопки в заголовке окна имеют следующие имена:<ul><li>Свести к минимуму</li><li>"Maximize" или "Restore",</li><li>"Close" (Закрыть)</li><li>"Контекстная Справка"</li><li>ВВОДА</li></ul> | 
| <strong>get_accParent</strong> | Свойство <strong>Parent</strong> заголовка окна является основным окном приложения ( <a href="object-roles.md"><strong>ROLE_SYSTEM_WINDOW</strong></a> ), которое имеет то же имя класса окон, что и заголовок окна приложения. | 
| <strong>get_accRole</strong> | Свойство <strong>Role</strong> имеет значение <a href="object-roles.md"><strong>ROLE_SYSTEM_TITLEBAR</strong></a>. Дочерние кнопки в строке заголовка имеют свойство <strong>Role</strong> <a href="object-roles.md"><strong>ROLE_SYSTEM_PUSHBUTTON</strong></a>. | 
| <strong>get_accState</strong> | Свойство <strong>State</strong> для заголовка окна и дочерних кнопок может быть сочетанием одного или нескольких из следующих <a href="object-state-constants.md">значений</a>: <a href="object-state-constants.md"><strong>STATE_SYSTEM_FOCUSABLE</strong></a> | <a href="object-state-constants.md"><strong>STATE_SYSTEM_INVISIBLE</strong></a> | <a href="object-state-constants.md"><strong>STATE_SYSTEM_OFFSCREEN</strong></a> | <a href="object-state-constants.md"><strong>STATE_SYSTEM_UNAVAILABLE</strong></a> | <a href="object-state-constants.md"><strong>STATE_SYSTEM_PRESSED</strong></a><br /> | 
| <strong>get_accValue</strong> | Свойство <strong>value</strong> — это строка, которая совпадает с текстом, отображаемым в заголовке окна. | 




 

## <a name="notes"></a>Примечания

-   Несмотря на то, что заголовок приложения имеет свойство **State** , которое имеет [**\_ \_ фокус системы состояния**](object-state-constants.md), оно никогда не имеет **отметок состояния** [**\_ системы \_**](object-state-constants.md). Установка фокуса на заголовке окна приложения помещается в главное окно.
-   Поскольку объект заголовка окна не поддерживает [**Get \_ аккчилд**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchild), кнопки в заголовке окна являются простыми элементами. Они не поддерживают интерфейс [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) сами по себе. Объект заголовка окна содержит сведения об этих дочерних кнопках.
-   Поскольку строки заголовка не получают фокус и не имеют действия по умолчанию, методы [**аккдодефаултактион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accdodefaultaction) и [**Get \_ аккдефаултактион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accdefaultaction) не поддерживаются для этого элемента управления.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Интерфейс IAccessible](/windows/desktop/api/oleacc/nn-oleacc-iaccessible)
</dt> </dl>

 

 





