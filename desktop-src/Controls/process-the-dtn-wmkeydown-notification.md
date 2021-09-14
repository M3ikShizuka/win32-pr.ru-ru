---
title: Обработка уведомления DTN_WMKEYDOWN
description: В этом разделе показано, как обработать \_ уведомление ДТН вмкэйдовн. Обработка этого кода уведомления позволяет владельцу элемента управления предоставлять определенные ответы на нажатия клавиш в полях обратного вызова элемента управления.
ms.assetid: CD521C62-CF52-4FFF-A598-E5EBA34471FB
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: cec97ffc5853743c357081b974d155ee0e0977d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167631"
---
# <a name="how-to-process-the-dtn_wmkeydown-notification"></a>Обработка \_ уведомления ДТН вмкэйдовн

В этом разделе показано, как обработать уведомление [ДТН \_ вмкэйдовн](dtn-wmkeydown.md) . Обработка этого кода уведомления позволяет владельцу элемента управления предоставлять определенные ответы на нажатия клавиш в полях обратного вызова элемента управления.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Instructions


Элементы управления "Выбор даты и времени" (DTP) отправляют сообщение [ \_ вмкэйдовн ДТН](dtn-wmkeydown.md) , чтобы сообщить о том, что пользователь ввел ввод в поле обратного вызова. Если вы хотите эмулировать те же ответы клавиатуры, которые поддерживаются для стандартных полей DTP или предоставляющих пользовательские ответы, приложение должно содержать код для работы с этим уведомлением.

Следующий пример кода C++ представляет собой определяемую приложением функцию, которая обрабатывает уведомление [ДТН \_ вмкэйдовн](dtn-wmkeydown.md) .

**Предупреждение системы безопасности:** Неправильное использование **лстркмп** может привести к нарушению безопасности приложения. Например, перед вызовом **лстркмп** в следующем примере кода следует убедиться, что две строки завершаются нулем. перед продолжением следует ознакомиться с [вопросами безопасности: элементы управления Microsoft Windows](sec-comctls.md) .



```C++
//  DoWMKeydown increments or decrements the day of month according 
//  to user keyboard input.

void WINAPI DoWMKeydown(
 HWND hwndDP,
 LPNMDATETIMEWMKEYDOWN lpDTKeystroke)
{
    int delta =1;
    if(!lstrcmp(lpDTKeystroke->pszFormat,L"XX")){
        switch(lpDTKeystroke->nVirtKey){
            case VK_DOWN:
            case VK_SUBTRACT:
                delta = -1;  // fall through

            case VK_UP:
            case VK_ADD:
                lpDTKeystroke->st.wDay += (WORD) delta;
                break;
        }
    }
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование элементов управления "Выбор даты и времени"](using-date-and-time-picker.md)
</dt> <dt>

[Справочник по элементу выбора даты и времени](bumper-date-and-time-picker-date-and-time-picker-control-reference.md)
</dt> <dt>

[Выбор даты и времени](date-and-time-picker-control-reference.md)
</dt> </dl>

 

 




