---
title: Использование групп в List-View
description: В этом разделе описывается создание экземпляра группы и его добавление в элемент управления "представление списка".
ms.assetid: 8486B9A2-C519-4912-9E88-3BAFCC4D51CF
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ec47d73c3e8b808eaf1909bdafb015c7eebc37de
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165415"
---
# <a name="how-to-use-groups-in-a-list-view"></a>Использование групп в List-View

В этом разделе описывается создание экземпляра группы и его добавление в элемент управления "представление списка". Группирование позволяет пользователю упорядочивать списки по группам элементов, которые визуально разделены на странице, с помощью горизонтального разделителя и заголовка группы.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Instructions


Чтобы использовать группы в элементе управления "представление списка", убедитесь, что элемент управления содержит стиль окна [**LVS \_ алигнтоп**](list-view-window-styles.md) .

При добавлении элемента в список его необходимо назначить группе, задав элемент **играупид** структуры [**лвитем**](/windows/win32/api/commctrl/ns-commctrl-lvitema) элемента в качестве значения элемента **играупид** структуры [**лвграуп**](/windows/win32/api/commctrl/ns-commctrl-lvgroup) в группах. Элемент, не назначенный группе, не отображается в списке, если включено представление группы. Чтобы включить или отключить представление группы, используйте макрос [**\_ енаблеграупвиев ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_enablegroupview) .

В следующем примере показано, как создать группу с заголовком и добавить ее в элемент управления "представление списка".


```C++
    LVGROUP group;

    group.cbSize    = sizeof(LVGROUP);
    group.mask      = LVGF_HEADER | LVGF_GROUPID;
    group.pszHeader = TEXT("Dogs");
    group.iGroupId  = 1;

    ListView_InsertGroup(hWndListView, -1, &group);

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по элементу управления представления списка](bumper-list-view-list-view-control-reference.md)
</dt> <dt>

[Сведения об элементах управления List-View](list-view-controls-overview.md)
</dt> <dt>

[Использование элементов управления List-View](using-list-view-controls.md)
</dt> </dl>

 

 




