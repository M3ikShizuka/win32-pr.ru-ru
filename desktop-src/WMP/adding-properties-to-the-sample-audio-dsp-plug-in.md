---
title: Добавление свойств в образец подключаемого модуля DSP для аудио
description: Добавление свойств в образец подключаемого модуля DSP для аудио
ms.assetid: 9c6c2a34-4844-476b-8814-a95a236e75bb
keywords:
- подключаемые модули проигрыватель Windows Media, DSP аудиоподсистемы
- подключаемые модули, DSP аудиоподсистемы
- подключаемые модули обработки цифровых сигналов, свойства аудио
- Подключаемые модули DSP, звуковые свойства
- подключаемые модули DSP аудио, свойства
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d180ab1054631b09997ac986529a641e6ff05ec3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374320"
---
# <a name="adding-properties-to-the-sample-audio-dsp-plug-in"></a>Добавление свойств в образец подключаемого модуля DSP для аудио

пример кода DSP, который создается мастером подключаемых модулей проигрыватель Windows Media, использует одно свойство, представляющее коэффициент масштабирования для звукового тома. Подключаемому модулю может потребоваться более одного свойства. вы можете легко добавить свойства в подключаемый модуль DSP в Visual Studio, выполнив следующие действия.

-   Определите методы в коде определения интерфейса в IDL-файле, который является частью проекта-заглушки.
    -   Добавьте реализации методов в основной файл CPP проекта:

    ```C++
    STDMETHODIMP CYourProject::get_color(COLORREF *pColor)
    {
        if ( NULL == pColor )
        {
            return E_POINTER;
        }

        *pColor = m_Color;

        return S_OK;
    }

    STDMETHODIMP CYourProject::put_color(COLORREF newColor)
    {
        m_Color = newColor;
        
        return S_OK;
    }
    
    ```

    

Наконец, чтобы сделать свойства доступными для пользователя, необходимо внести изменения в реализацию страницы свойств.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Реализация подключаемого модуля DSP аудиоподсистемы**](implementing-an-audio-dsp-plug-in.md)
</dt> </dl>

 

 




