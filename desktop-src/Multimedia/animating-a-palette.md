---
title: Анимация палитры
description: Анимация палитры
ms.assetid: 89493cc3-eca9-407f-99c2-903fba16992c
keywords:
- Дравдиб, палитры
- Функция Дравдибреализе
- Функция Дравдибдрав
- Функция Дравдибчанжепалетте
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e023ba8ee2c4791ebc8c3f2ac7ebf9a198f4a5ae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055249"
---
# <a name="animating-a-palette"></a>Анимация палитры

В следующем примере палитра анимируется с помощью функций [**дравдибреализе**](/windows/desktop/api/Vfw/nf-vfw-drawdibrealize), [**дравдибчанжепалетте**](/windows/desktop/api/Vfw/nf-vfw-drawdibchangepalette)и [**дравдибдрав**](/windows/desktop/api/Vfw/nf-vfw-drawdibdraw) .

Цвета точечного рисунка можно изменить с помощью функции [**дравдиббегин**](/windows/desktop/api/Vfw/nf-vfw-drawdibbegin) в сочетании с [**дравдибчанжепалетте**](/windows/desktop/api/Vfw/nf-vfw-drawdibchangepalette). Во – первых, чтобы разрешить изменение палитры, укажите \_ флаг анимации DDF в вызове **дравдиббегин**. Во вторых, задайте значения цветовой таблицы из записей палитры с помощью **дравдибчанжепалетте**.

Например, если *лппе* является адресом массива [палеттинтри](/previous-versions//ms532623(v=vs.85)) , содержащего новые цвета, а *лпби* является структурой [**Битмапинфохеадер**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfoheader) , используемой в [**ДРАВДИББЕГИН**](/windows/desktop/api/Vfw/nf-vfw-drawdibbegin) или [**дравдибдрав**](/windows/desktop/api/Vfw/nf-vfw-drawdibdraw), следующий фрагмент обновляет таблицу цветов DIB.


```C++
hdc = GetDC(hwnd); 
DrawDibBegin(hdd, ....., DDF_ANIMATE); 
DrawDibRealize(hdd, hdc, fBackground); 
DrawDibDraw(hdd, hdc, ...., DDF_SAME_DRAW|DDF_SAME_HDC); 
 
// Call to change color. 
DrawDibChangePalette(hDD, iStart, iLen, lppe); 
. 
. 
. 
ReleaseDC(hwnd, hdc); 

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование Дравдиб](using-drawdib.md)
</dt> </dl>

 

 