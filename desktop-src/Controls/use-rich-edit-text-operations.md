---
title: Как использовать широкие операции редактирования текста
description: Приложение может отсылать сообщения для получения или поиска текста в элементе управления Rich Edit. Можно получить выделенный текст или указанный фрагмент текста.
ms.assetid: 95D88F9A-3DD1-48E4-B6FF-3168F2D25846
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 91018dfd2c13c589530b9e3d5abe5399a8128bb5904e66c5aceacb692ae0d0ee
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120132084"
---
# <a name="how-to-use-rich-edit-text-operations"></a>Как использовать широкие операции редактирования текста

Приложение может отсылать сообщения для получения или поиска текста в элементе управления Rich Edit. Можно получить выделенный текст или указанный фрагмент текста.

Чтобы получить выделенный текст в элементе управления Rich Edit, используйте сообщение [**EM \_ жетселтекст**](em-getseltext.md) . Текст копируется в указанный массив символов. Необходимо убедиться, что массив достаточно велик, чтобы вместить выделенный текст, а также завершающий нуль-символ.

Чтобы получить указанный диапазон текста, используйте сообщение [**EM \_ жеттекстранже**](em-gettextrange.md) . Структура [**TEXTRANGE**](/windows/win32/api/richedit/ns-richedit-textrangea) , используемая с этим сообщением, указывает диапазон текста для извлечения и указывает на массив символов, который получает текст. В этом случае приложение должно обеспечить достаточно большой размер массива для указанного текста и завершающего нуль-символа.

Вы можете выполнять поиск строки в элементе управления Rich Edit с помощью сообщений [**EM \_ строки FindText**](em-findtext.md) или [**EM \_ финдтекстекс**](em-findtextex.md) или их эквивалентов в Юникоде, [**EM \_ финдтекств**](em-findtextw.md) и [**EM \_ финдтекстексв**](em-findtextexw.md). Структура [**строки FindText**](/windows/win32/api/richedit/ns-richedit-findtexta) , используемая с нерасширенными версиями, задает текстовый диапазон для поиска и искомую строку. В расширенных версиях используется структура [**финдтекстекс**](/windows/desktop/api/Richedit/ns-richedit-findtextexa) , которая задает одни и те же сведения, а также начальную и конечную точки диапазона символов найденного текста. Можно также указать такие параметры, как при поиске с учетом регистра.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Инструкции

### <a name="use-a-rich-edit-text-operation"></a>Использование операции расширенного ввода текста

Следующий пример функции находит указанный текст в выделенном тексте в элементе управления Rich Edit, поддерживающем Юникод. Если целевой объект найден, он становится новым выбором.


```C++
BOOL FindTextInSelection(HWND hRich, WCHAR* target)
{
    CHARRANGE selectionRange;
    
    SendMessage(hRich, EM_EXGETSEL, 0, (LPARAM)&selectionRange);
    
    FINDTEXTEX ftex;
    
    ftex.lpstrText  = target;
    ftex.chrg.cpMin = selectionRange.cpMin;
    ftex.chrg.cpMax = selectionRange.cpMax;
    
    LRESULT lr = SendMessage(hRich, EM_FINDTEXTEXW, (WPARAM)FR_DOWN, (LPARAM) &ftex);
    
    if (lr >= 0)
    {
        LRESULT lr1 = SendMessage(hRich, EM_EXSETSEL, 0, (LPARAM)&ftex.chrgText);
        
        SendMessage(hRich, EM_HIDESELECTION, (LPARAM)FALSE, 0);
        
        return TRUE;
    }
    
    return FALSE;
    
}
```



## <a name="remarks"></a>Remarks

Microsoft Rich Edit 3,0 также поддерживает функцию редактора метода ввода (IME) Хекстауникоде, позволяющую пользователю выполнять преобразование между шестнадцатеричными и Юникод с помощью горячих клавиш. Дополнительные сведения см. в разделе [ХЕКСТАУНИКОДЕ IME](/windows/desktop/Intl/hextounicode-ime).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование элементов управления Rich Edit](using-rich-edit-controls.md)
</dt> <dt>

[демонстрация Windows стандартных элементов управления (кппвиндовскоммонконтролс)](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/master/OneCodeTeam/Windows%20common%20controls%20demo%20(CppWindowsCommonControls)/%5BC++%5D-Windows%20common%20controls%20demo%20(CppWindowsCommonControls)/C++/CppWindowsCommonControls)
</dt> </dl>

 

 