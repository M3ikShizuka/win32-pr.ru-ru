---
title: Ограничение перемещения ползунка
description: Как описано в разделе о элементах управления TrackBar, можно отключить часть диапазона TrackBar в качестве диапазона выбора. Одной из целей диапазона выбора может быть ограничение перемещения ползунка, что делает некоторые части ограничений полного диапазона.
ms.assetid: 9DD8BB11-EC6F-4695-BA56-5061F6EA5436
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4faf4a88f95ec521330e9084eef66f29b2f5d872c1f6375020b1d4519cf64e25
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120085154"
---
# <a name="how-to-limit-slider-movement"></a>Ограничение перемещения ползунка

Как описано в разделе [о элементах управления TrackBar](trackbar-controls.md), можно отключить часть диапазона TrackBar в качестве диапазона выбора. Одной из целей диапазона выбора может быть ограничение перемещения ползунка, что делает некоторые части ограничений полного диапазона.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Инструкции

### <a name="limit-slider-movement"></a>Ограничение перемещения ползунка

В следующем примере кода ограничивается перемещение ползунка путем сброса положения ползунка при перемещении за пределы диапазона выбора.


```
case WM_HSCROLL:
    {
        HWND hTrackbar = GetDlgItem(hDlg, IDC_SLIDER1);
        
        if (hTrackbar == (HWND)lParam)
        {
            int newPos    = SendMessage(hTrackbar, TBM_GETPOS, 0, 0);
            int selStart  = SendMessage(hTrackbar, TBM_GETSELSTART, 0, 0);
            int selEnd    = SendMessage(hTrackbar, TBM_GETSELEND, 0, 0);
            
            if (newPos > selEnd)
            {
                SendMessage(hTrackbar, TBM_SETPOS, (WPARAM)TRUE, (LPARAM)selEnd);
            }
            
            else if (newPos < selStart)
            {
                SendMessage(hTrackbar, TBM_SETPOS, (WPARAM)TRUE, (LPARAM)selStart);
            }
        }
        
        break;
    }
```



## <a name="remarks"></a>Remarks

Этот фрагмент кода был бы частью процедуры окна диалогового окна.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование элементов управления TrackBar](using-trackbar-controls.md)
</dt> </dl>

 

 




