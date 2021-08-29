---
title: Создание элемента управления "IP-адрес"
description: В этом разделе показано, как создать экземпляр элемента управления IP-адреса.
ms.assetid: E4DBECA6-B3F2-405F-8D95-32FA2334114D
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 308893b436760ad970025b93d49a368fa44b28c7913c433ff4febad105cc41b6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120063114"
---
# <a name="how-to-create-an-ip-address-control"></a>Создание элемента управления "IP-адрес"

В этом разделе показано, как создать экземпляр элемента управления IP-адреса.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Инструкции


Перед созданием элемента управления IP-адресом загрузите библиотеку DLL общих элементов управления, вызвав [**InitCommonControlsEx**](/windows/desktop/api/Commctrl/nf-commctrl-initcommoncontrolsex). Затем используйте [**CreateWindow**](/windows/desktop/api/winuser/nf-winuser-createwindowa) или функцию [**CreateWindowEx**](/windows/desktop/api/winuser/nf-winuser-createwindowexa) для создания элемента управления IP-адреса экземпляра. Имя класса для элемента управления — [**WC \_ IPAddress**](common-control-window-classes.md). Используйте стиль [**\_ дочерний элемент WS**](/windows/desktop/winmsg/window-styles) , так как нет определенной константы стиля, связанной с элементом управления IP-адреса.

В следующем примере кода C++ функция, определяемая приложением, сначала вызывает [**InitCommonControlsEx**](/windows/desktop/api/Commctrl/nf-commctrl-initcommoncontrolsex) и устанавливает для элемента **двикк** структуры [**InitCommonControlsEx**](/windows/win32/api/commctrl/ns-commctrl-initcommoncontrolsex) значение [**ICC-классов в \_ Интернете \_**](/windows/win32/api/commctrl/ns-commctrl-initcommoncontrolsex), которое указывает класс IP Address. Затем он вызывает [**CreateWindowEx**](/windows/desktop/api/winuser/nf-winuser-createwindowexa) для создания экземпляра элемента управления IP-адреса.


```C++
// CreateIPAdressFld - creates a IPAddress control.
// Returns the handle to the new control
// TO DO:  calling procedure needs to check whether the handle is NULL, in case 
// of an error in creation.
// int xcoord, ycoord the coordinates of location of the control in the parent window
// HINST hInst is the global handle to the application instance.
// HWND  hWndParent is the handle to the control's parent window. 
//
//
HWND CreateIPAddressFld (HWND hwndParent, int xcoord, int ycoord) 
{     
     
    INITCOMMONCONTROLSEX icex;
    
    // Ensure that the common control DLL is loaded. 
    icex.dwSize = sizeof(INITCOMMONCONTROLSEX);
    icex.dwICC  = ICC_INTERNET_CLASSES ;
    InitCommonControlsEx(&icex); 
    
    // Create the IPAddress control.        
    HWND hWndIPAddressFld = CreateWindow(WC_IPADDRESS, 
                                L"", 
                                WS_CHILD | WS_OVERLAPPED | WS_VISIBLE, 
                                xcoord, 
                                ycoord,
                                150, 
                                20,  
                                hwndParent, 
                                NULL, 
                                hInst, 
                                NULL); 
                                
    return (hWndIPAddressFld);
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по управлению IP-адресами](bumper-ip-address-control-ip-address-control-reference.md)
</dt> <dt>

[Сведения об элементах управления IP-адресов](ip-address-controls.md)
</dt> <dt>

[Использование элементов управления IP-адресами](using-ip-address-controls.md)
</dt> </dl>

 

 