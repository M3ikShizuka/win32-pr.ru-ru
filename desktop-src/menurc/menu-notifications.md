---
title: Уведомления меню
description: Уведомления меню
ms.assetid: 8ff5671e-a666-483c-9ac1-f8be6eb58ffa
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f593e3007dff82241dc9e917a6cfa140cc443679
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127268520"
---
# <a name="menu-notifications"></a>Уведомления меню

## <a name="in-this-section"></a>в этом разделе

-   [**\_команда WM**](wm-command.md)
-   [**WM \_ CONTEXTMENU**](wm-contextmenu.md)
-   [**WM \_ ентерменулуп**](wm-entermenuloop.md)
-   [**WM \_ екситменулуп**](wm-exitmenuloop.md)
-   [**WM \_ жеттитлебаринфоекс**](wm-gettitlebarinfoex.md)
-   [**WM \_ MENUCOMMAND**](wm-menucommand.md)
-   [**WM \_ менудраг**](wm-menudrag.md)
-   [**WM \_ менужетобжект**](wm-menugetobject.md)
-   [**WM \_ менурбуттонуп**](wm-menurbuttonup.md)
-   [**WM \_ некстмену**](wm-nextmenu.md)
-   [**WM \_ унинитменупопуп**](wm-uninitmenupopup.md)


## <a name="example"></a>Пример

```c
BOOL AboutDlg (
    HWND hDlg, 
    UINT message, 
    WPARAM wParam, 
    LPARAM lParam)
{
    BOOL bRet = FALSE;
    
    switch (message) 
    {
        case WM_INITDIALOG:
            bRet = TRUE;
            break;

        case WM_COMMAND:
            if (wParam == IDOK ||
                wParam == IDCANCEL) 
            {
                EndDialog(hDlg, TRUE);
                bRet = TRUE;
            }
            break;
    }

    return bRet;
}
```
пример, взятый из [классической выборки Windows](https://github.com/microsoft/Windows-classic-samples) на GitHub.

 




