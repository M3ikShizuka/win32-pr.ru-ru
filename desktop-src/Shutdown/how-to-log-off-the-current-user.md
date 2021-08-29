---
description: В следующем примере функция Екситвиндовс используется для выхода текущего пользователя из системы.
ms.assetid: 74be3505-c4bd-4ae2-aaed-700382839006
title: Выход из системы текущего пользователя
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 029f7b1a68973f248162871572284a2dd20ffaaf34618a7e986035abf5f78f89
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119664384"
---
# <a name="how-to-log-off-the-current-user"></a>Выход из системы текущего пользователя

В следующем примере функция [**екситвиндовс**](/windows/desktop/api/Winuser/nf-winuser-exitwindows) используется для выхода текущего пользователя из системы.

``` syntax
// Log off the current user. 

ExitWindows(0, 0);
```

В следующем примере функция [**ExitWindowsEx**](/windows/desktop/api/Winuser/nf-winuser-exitwindowsex) используется для выхода текущего пользователя из системы.

``` syntax
// Log off the current user. 

ExitWindowsEx(EWX_LOGOFF, 0);
```

Приложение получает сообщение [**WM \_ куерендсессион**](wm-queryendsession.md) и отображает диалоговое окно с просьбой подтвердить завершение сеанса. Если пользователь нажмет кнопку **Да**, система выполнит выход пользователя из системы. Если пользователь нажмет кнопку **нет**, выход из системы отменяется.

``` syntax
// Process the message in the window procedure. 

case WM_QUERYENDSESSION:  
{ 
    int r; 
    r = MessageBox(NULL,(LPCWSTR)L"End the session?",(LPCWSTR)L"WM_QUERYENDSESSION",MB_YESNO);
 
    // Return TRUE to continue, FALSE to stop. 
 
    return r == IDYES; 
    break; 
}
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Выход из системы](logging-off.md)
</dt> </dl>

 

 



