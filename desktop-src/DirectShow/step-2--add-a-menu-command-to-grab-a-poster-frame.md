---
description: Шаг 2. Добавление команды меню для захвата афиши
ms.assetid: 9a0f807b-5543-41d4-ad2a-030a4346131c
title: Шаг 2. Добавление команды меню для захвата афиши
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f282ba112a9035edd9e75c9ea28709ec9c5dc137562ec75dbc5121de04dad864
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119650904"
---
# <a name="step-2-add-a-menu-command-to-grab-a-poster-frame"></a>Шаг 2. Добавление команды меню для захвата афиши

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

В этом разделе приводится шаг 2 по [извлечению кадра афиши](grabbing-a-poster-frame.md).

Затем добавьте команду для пользователя, чтобы взять афишу из файла. Создайте пункт меню с ИДЕНТИФИКАТОРом ресурса \_ точечного рисунка IDM и добавьте в процедуру окна следующую инструкцию CASE:


```C++
case WM_COMMAND:
    switch (LOWORD(wparam))
    {
    case IDM_BITMAP:
        {
            HRESULT hr = DoShowBitmap(hwnd, &pbmi);
            if (SUCCEEDED(hr))
            {
                pBuffer = reinterpret_cast<BYTE*>(pbmi) + 
                    sizeof(BITMAPINFOHEADER);
                InvalidateRect(hwnd, NULL, TRUE);
            }
            else
            {
                MessageBox(hwnd, TEXT("Cannot display the image."),
                    TEXT("Error"), MB_OK | MB_ICONERROR);
            }
        }
        break;  // IDM_BITMAP
    }
    break;  // WM_COMMAND
```



Функция Дошовбитмап вернет выделенный буфер в *пбми*. При условии, что функция выполнена, адрес точечного рисунка (


```C++
pBuffer
```



) можно вычислить как смещение от *пбми*. В функции Дошовбитмап выведите диалоговое окно **Открыть файл** , чтобы пользователь выбрал файл, а затем вызовите функцию, определяемую приложением, которая будет извлекать точечный рисунок:


```C++
HRESULT DoShowBitmap(HWND hwnd, BITMAPINFOHEADER** ppbmih)
{
    OPENFILENAME ofn;       // common dialog box structure
    // Initialize OPENFILENAME (not shown).
    // Display the Open File dialog box.  
    if (GetOpenFileName(&ofn) != TRUE) // failed to open file
    {
        return E_FAIL;
    }
    return GetBitmap(ofn.lpstrFile, ppbmih);
}
```



Далее. [Шаг 3. Реализация функции Frame-Grabbing](step-3--implement-the-frame-grabbing-function.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Зафрагментировать рамку афиши](grabbing-a-poster-frame.md)
</dt> </dl>

 

 



