---
title: Создание кнопки
description: Для динамического создания кнопок используется функция CreateWindow или CreateWindowEx. В этом разделе показано, как использовать функцию CreateWindow для создания кнопки отправки по умолчанию.
ms.assetid: A8C56D09-90A3-4C70-9907-61390521D1DA
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c4940016eaab8f64cd82f18579b31b13f2835ab8a0de00752eabfe81da316d6d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119920924"
---
# <a name="how-to-create-a-button"></a>Создание кнопки

Для динамического создания кнопок используется функция [**CreateWindow**](/windows/desktop/api/winuser/nf-winuser-createwindowa) или [**CreateWindowEx**](/windows/desktop/api/winuser/nf-winuser-createwindowexa) . В этом разделе показано, как использовать функцию **CreateWindow** для создания кнопки отправки по умолчанию.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Инструкции


Используйте функцию [**CreateWindow**](/windows/desktop/api/winuser/nf-winuser-createwindowa) для создания элемента управления "Кнопка".

В следующем примере C++ параметр *m \_ HWND* является дескриптором родительского окна. Стиль " [**BS \_ дефпушбуттон**](button-styles.md) " указывает, что должна быть создана кнопка принудительной установки по умолчанию. Обратите внимание, что значения размера и расположения должны быть заданы, так как при использовании **\_ Уседефаулт во Вт** . для кнопки устанавливаются нулевые значения.


```C++
HWND hwndButton = CreateWindow( 
    L"BUTTON",  // Predefined class; Unicode assumed 
    L"OK",      // Button text 
    WS_TABSTOP | WS_VISIBLE | WS_CHILD | BS_DEFPUSHBUTTON,  // Styles 
    10,         // x position 
    10,         // y position 
    100,        // Button width
    100,        // Button height
    m_hwnd,     // Parent window
    NULL,       // No menu.
    (HINSTANCE)GetWindowLongPtr(m_hwnd, GWLP_HINSTANCE), 
    NULL);      // Pointer not needed.
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[О кнопках](about-buttons.md)
</dt> <dt>

[Справочник по элементу управления Button](bumper-button-button-control-reference.md)
</dt> <dt>

[Использование кнопок](using-buttons.md)
</dt> <dt>

[Кнопка](buttons.md)
</dt> </dl>

 

 