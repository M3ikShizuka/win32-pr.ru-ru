---
title: Рисование контекста отображения
description: Рисование контекста отображения
ms.assetid: c3328375-faa3-4b29-a155-8a25cc62269f
keywords:
- Дравдиб, контекст устройства (DC)
- Дравдиб, рисование контроллеров доменов
- Функция Дравдибреализе
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ef1c79c2b7bb938cc34527b23cfc66fda6d19503
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371859"
---
# <a name="drawing-a-display-context"></a>Рисование контекста отображения

В следующем примере подготавливается контроллер домена Дравдиб с помощью функции [**дравдибреализе**](/windows/desktop/api/Vfw/nf-vfw-drawdibrealize) до отображения нескольких изображений в последовательности точечных рисунков.


```C++
hdc = GetDC(hwnd); 
DrawDibBegin(hdd, hdc, dxDest, dyDest, lpbi, dxSrc, dySrc, NULL); 
DrawDibRealize(hdd, hdc, fBackground); 
DrawDibDraw(hdd, hdc, xDst, yDst, dxDst, dyDst, lpbi, lpBits, 
    xSrc, ySrc, dxSrc, dySrc, DDF_SAME_DRAW|DDF_SAME_HDC); 
DrawDibDraw(hdd, hdc, xDst, yDst, dxDst, dyDst, lpbi, lpBits, 
    xSrc, ySrc, dxSrc, dySrc, DDF_SAME_DRAW|DDF_SAME_HDC); 
DrawDibDraw(hdd, hdc, xDst, yDst, dxDst, dyDst, lpbi, lpBits, 
    xSrc, ySrc, dxSrc, dySrc, DDF_SAME_DRAW|DDF_SAME_HDC); 
ReleaseDC(hwnd, hdc); 

```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Использование Дравдиб](using-drawdib.md)
</dt> </dl>

 

 




