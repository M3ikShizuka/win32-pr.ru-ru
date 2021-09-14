---
title: Форматирование и макет текста
description: DirectWrite предоставляет два интерфейса для форматирования text идвритетекстформат и идвритетекстлайаут.
ms.assetid: a68963a6-e486-4881-8ad6-873173396fca
keywords:
- DirectWrite, форматирование текста
- DirectWrite, макет
- DirectWrite, интерфейс идвритетекстформат
- DirectWrite, интерфейс идвритетекстлайаут
- Интерфейс Идвритетекстформат
- Интерфейс Идвритетекстлайаут
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e9e5790742a3d3caf7f962a6b5e2b3111c626f28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057927"
---
# <a name="text-formatting-and-layout"></a>Форматирование и макет текста

[DirectWrite](direct-write-portal.md) предоставляет два интерфейса для форматирования текста: [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) и [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout). **Идвритетекстформат** описывает только формат текста и используется в тех случаях, когда вся строка имеет одинаковый размер, стиль, вес и т. д. С другой стороны, **идвритетекстлайаут** инкапсулирует текстовую строку и форматирование для указанных диапазонов строки. В этом документе описывается каждый интерфейс и их использование. Дополнительные сведения о создании и методах этих интерфейсов см. на страницах справочника по [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) и [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) .

Этот документ содержит следующие компоненты:

-   [идвритетекстформат](#modifying-an-idwritetextformat)
    -   [Изменение Идвритетекстформат](#modifying-an-idwritetextformat)
-   [идвритетекстлайаут](#idwritetextlayout)
    -   [Форматирование диапазона текста](#formatting-a-range-of-text)
    -   [Параметры подготовки к просмотру](#rendering-options)

## <a name="idwritetextformat"></a>идвритетекстформат

Объект [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) используется для:

-   Опишите формат всей строки при подготовке к просмотру. Чтобы отобразить строку с несколькими форматами, используйте объект [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) .
-   При создании объекта [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) укажите формат текста по умолчанию.

Чтобы создать объект [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) , используйте метод [**Идвритефактори:: креатетекстформат**](/windows/win32/api/dwrite/nf-dwrite-idwritefactory-createtextformat) и укажите семейство шрифтов, коллекцию шрифтов, плотность шрифта, размер шрифта (в DIP), имя локали.

### <a name="modifying-an-idwritetextformat"></a>Изменение Идвритетекстформат

После создания интерфейса [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) некоторые значения не могут быть изменены: семейство шрифтов, коллекция, вес и размер, а также имя локали. Чтобы изменить эти значения, необходимо создать новый объект **идвритетекстформат** .

[**Идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) позволяет изменить приведенные выше свойства, не создавая ничего. [**Идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) позволяет вносить изменения формата, применяемые ко всему тексту, например выравнивание текста. Если вы хотите применить форматирование к конкретным диапазонам символов, это следует сделать с помощью **идвритетекстлайаут**.

[**Идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) предоставляет методы для задания выравнивания текста, направления потока, инкрементной табуляции, интервала между строками, выравнивания абзаца, обрезки и переноса слов. Эти свойства можно изменить в любое время после создания объекта **идвритетекстформат** .

## <a name="idwritetextlayout"></a>идвритетекстлайаут

Интерфейс [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) , в отличие от [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat), представляет как блок текста, так и связанное форматирование. **Идвритетекстформат** представляет сведения о начальном форматировании. В следующем примере показано, как создать объект **идвритетекстлайаут** с помощью [**Идвритефактори:: креатетекстлайаут**](/windows/win32/api/dwrite/nf-dwrite-idwritefactory-createtextlayout).


```C++
// Create a text layout using the text format.
if (SUCCEEDED(hr))
{
    RECT rect;
    GetClientRect(hwnd_, &rect); 
    float width  = rect.right  / dpiScaleX_;
    float height = rect.bottom / dpiScaleY_;

    hr = pDWriteFactory_->CreateTextLayout(
        wszText_,      // The string to be laid out and formatted.
        cTextLength_,  // The length of the string.
        pTextFormat_,  // The text format to apply to the string (contains font information, etc).
        width,         // The width of the layout box.
        height,        // The height of the layout box.
        &pTextLayout_  // The IDWriteTextLayout interface pointer.
        );
}

```



Текст в объекте [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) не может быть изменен после создания объекта. Чтобы изменить текст, необходимо удалить существующий объект и создать новый объект **идвритетекстлайаут** .

Для форматирования указанных диапазонов текста можно использовать [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) . **Идвритетекстлайаут** также предоставляет методы для изменения стиля и веса шрифта и добавления функций шрифтов OpenType и проверки попадания. Дополнительные сведения и полный список методов см. на странице справочника по [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) .

### <a name="formatting-a-range-of-text"></a>Форматирование диапазона текста

[**Идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) предоставляет несколько методов для форматирования диапазонов текста. Каждый из этих методов принимает в качестве параметра структуру [**\_ \_ диапазона текста дврите**](/windows/win32/api/dwrite/ns-dwrite-dwrite_text_range) , чтобы указать начальную текстовую точку в строке и длину диапазона для форматирования. В следующем примере показано, как задать полужирным шрифтом начертание шрифта для диапазона текста.


```C++
// Set the font weight to bold for the first 5 letters.
DWRITE_TEXT_RANGE textRange = {0, 5};

if (SUCCEEDED(hr))
{
    hr = pTextLayout_->SetFontWeight(DWRITE_FONT_WEIGHT_BOLD, textRange);
}

```



### <a name="rendering-options"></a>Параметры подготовки к просмотру

Текст с форматированием, описанным только в объекте [**идвритетекстформат**](/windows/win32/api/dwrite/nn-dwrite-idwritetextformat) , может быть визуализирован с помощью [Direct2D](../direct2d/direct2d-portal.md), однако существует несколько дополнительных параметров для отрисовки объекта [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) .

Строку, описываемую объектом [**идвритетекстлайаут**](/windows/win32/api/dwrite/nn-dwrite-idwritetextlayout) , можно визуализировать с помощью методов, приведенных ниже.

1.  [Прорисовка с помощью Direct2D](rendering-by-using-direct2d.md).
2.  [Отрисовка с помощью пользовательского модуля подготовки текста](how-to-implement-a-custom-text-renderer.md).
3.  [Подготовка к просмотру на поверхности GDI](render-to-a-gdi-surface.md).

 

 
