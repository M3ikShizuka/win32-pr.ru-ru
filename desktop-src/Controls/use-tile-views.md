---
title: Использование мозаичных представлений
description: В этом разделе показано, как задать мозаичное представление для элемента управления "представление списка".
ms.assetid: BDE17F4B-3A15-48BB-8160-036AD0DC3B41
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 616a9bb8a2c1707d903f0ebe2b6de86511dc6ce4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165380"
---
# <a name="how-to-use-tile-views"></a>Использование мозаичных представлений

В этом разделе показано, как задать мозаичное представление для элемента управления "представление списка". В мозаичном представлении каждый элемент представлен крупным значком с одной или несколькими строками сопроводительного текста. Иллюстрации см. в разделе [About List-View Controls](list-view-controls-overview.md).

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Instructions


Задайте общие параметры отображения для мозаичного представления с помощью макроса [**\_ сеттилевиевинфо ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_settileviewinfo) . Используйте структуру [**лвтилевиевинфо**](/windows/win32/api/commctrl/ns-commctrl-lvtileviewinfo) , переданную в этот макрос, чтобы указать расположение текста относительно значка, размер каждой плитки (включая сопроводительный текст) и максимальное число строк текста.

Если вы не хотите, чтобы размеры плиток автоматически изменялись, необходимо задать **лвтвиф \_ FIXEDSIZE** в элементе **dwFlags** и **лвтвим \_ тилесизе** в **Двмаск лвтилевиевинфо** , [**а**](/windows/win32/api/commctrl/ns-commctrl-lvtileviewinfo)также предоставить измерения в элементе **сизетиле** .

Следующий пример кода C++ устанавливает сведения о мозаичном представлении для элемента управления "представление списка", чтобы для каждого элемента отображалось не более двух подэлементов. Он также задает размер каждой плитки.


```C++
    SIZE size = { 100, 50 };
    LVTILEVIEWINFO tileViewInfo = {0};

    tileViewInfo.cbSize   = sizeof(tileViewInfo);
    tileViewInfo.dwFlags  = LVTVIF_FIXEDSIZE;
    tileViewInfo.dwMask   = LVTVIM_COLUMNS | LVTVIM_TILESIZE;
    tileViewInfo.cLines   = 2;
    tileViewInfo.sizeTile = size;

    ListView_SetTileViewInfo(hWndListView, &tileViewInfo);

```



Для каждого элемента в списке можно задать дополнительные параметры при вставке элемента в список или позже. Структура [**лвитем**](/windows/win32/api/commctrl/ns-commctrl-lvitema) , используемая с [**ListView \_ InsertItem**](/windows/desktop/api/Commctrl/nf-commctrl-listview_insertitem) , содержит члены, указывающие, какие столбцы данных должны отображаться под элементом, и их выравнивание. Эти же параметры вывода также находятся в структуре [**лвтилеинфо**](/windows/win32/api/commctrl/ns-commctrl-lvtileinfo) , используемой с [**ListView \_ сеттилеинфо**](/windows/desktop/api/Commctrl/nf-commctrl-listview_settileinfo).

> [!Note]  
> Здесь "Columns" означает не отображать столбцы в мозаичном представлении, а не подэлементы, отображаемые в столбцах в представлении сведений.

 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по элементу управления представления списка](bumper-list-view-list-view-control-reference.md)
</dt> <dt>

[Сведения об элементах управления List-View](list-view-controls-overview.md)
</dt> <dt>

[Использование элементов управления List-View](using-list-view-controls.md)
</dt> </dl>

 

 




