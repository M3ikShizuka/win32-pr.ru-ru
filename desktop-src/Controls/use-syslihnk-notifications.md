---
title: Как использовать уведомления SysLink
description: Существует два сообщения с уведомлениями, связанные с элементом управления SysLink \ 8212; один для мыши (NM \_ Click (Syslink)), а второй для клавиатуры (NM \_ Return).
ms.assetid: 77E80EB2-180B-4EDD-9FB5-9930E8886CA6
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2fb8a3c8f0f589e17e6fe413b8232876e131734aa053b9a091b83e7d94b14b7d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120132064"
---
# <a name="how-to-use-syslink-notifications"></a>Как использовать уведомления SysLink

С элементом управления SysLink связаны два сообщения уведомления: один для мыши ([NM \_ Click (Syslink)](nm-click-syslink.md)) и один для клавиатуры ([NM \_ return](nm-return.md)).

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Инструкции

### <a name="use-syslink-notifications"></a>Использование уведомлений SysLink

В следующем примере кода показано, как обрабатывать уведомления SysLink, которые создаются, когда пользователь щелкает одну из двух ссылок в [предыдущем примере](create-syslink-controls.md). Когда пользователь щелкает URL-адрес в Интернете, связанная веб-страница открывается в браузере по умолчанию. Когда пользователь щелкает гиперссылку, определяемую приложением, отображается окно сообщения.


```C++
// g_hLink is the handle of the SysLink control.
case WM_NOTIFY:

    switch (((LPNMHDR)lParam)->code)
    {
    
    case NM_CLICK:          // Fall through to the next case.
    
    case NM_RETURN:
        {
            PNMLINK pNMLink = (PNMLINK)lParam;
            LITEM   item    = pNMLink->item;
            
            if ((((LPNMHDR)lParam)->hwndFrom == g_hLink) && (item.iLink == 0))
              {
                ShellExecute(NULL, L"open", item.szUrl, NULL, NULL, SW_SHOW);
              }
            
            else if (wcscmp(item.szID, L"idInfo") == 0)
              {
                MessageBox(hDlg, L"This isn't much help.", L"Example", MB_OK);
              }
            
            break;
        }
    }
    
    break;
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование элементов управления SysLink](using-syslink-controls.md)
</dt> <dt>

[демонстрация Windows стандартных элементов управления (кппвиндовскоммонконтролс)](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/master/OneCodeTeam/Windows%20common%20controls%20demo%20(CppWindowsCommonControls)/%5BC++%5D-Windows%20common%20controls%20demo%20(CppWindowsCommonControls)/C++/CppWindowsCommonControls)
</dt> </dl>

 

 




