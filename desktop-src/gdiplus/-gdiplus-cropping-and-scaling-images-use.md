---
title: обрезка и масштабирование GDI+ изображений
description: Класс Graphics предоставляет несколько методов DrawImage, некоторые из которых имеют параметры исходного и целевого прямоугольника, которые можно использовать для кадрирования и масштабирования изображений.
ms.assetid: cad64615-d8e6-4c03-a6c7-c98267a8f159
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 18c70a7b4f7aa0374602326ab856a01bbadc0047
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580043"
---
# <a name="cropping-and-scaling-gdi-images"></a>обрезка и масштабирование GDI+ изображений

Класс [**Graphics**](/windows/desktop/api/gdiplusgraphics/nl-gdiplusgraphics-graphics) предоставляет несколько методов **DrawImage** , некоторые из которых имеют параметры исходного и целевого прямоугольника, которые можно использовать для кадрирования и масштабирования изображений.

В следующем примере объект [**Image**](/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-image) создается на основе файла Apple.gif. Код рисует все изображение Apple в исходном размере. Затем код вызывает метод **DrawImage** объекта [**Graphics**](/windows/desktop/api/gdiplusgraphics/nl-gdiplusgraphics-graphics) для рисования части изображения Apple в прямоугольнике назначения, который больше, чем исходный образ Apple.

Метод **DrawImage** определяет, какая часть Apple будет рисовать, просматривая исходный прямоугольник, который задается третьим, четвертым, пятый и шестым аргументами. В этом случае Apple обрезается до 75 процентов от его ширины и 75 процентов от высоты.

Метод **DrawImage** определяет, где следует нарисовать обрезанный Apple, а также размер обрезкиного Apple, просмотрев прямоугольник назначения, который задается вторым аргументом. В этом случае размер прямоугольника назначения составляет 30%, а высота составляет 30 процентов от исходного изображения.


```
Image image(L"Apple.gif");
UINT width = image.GetWidth();
UINT height = image.GetHeight();
// Make the destination rectangle 30 percent wider and
// 30 percent taller than the original image.
// Put the upper-left corner of the destination
// rectangle at (150, 20).
Rect destinationRect(150, 20, 1.3 * width, 1.3 * height);
// Draw the image unaltered with its upper-left corner at (0, 0).
graphics.DrawImage(&image, 0, 0);
// Draw a portion of the image. Scale that portion of the image
// so that it fills the destination rectangle.
graphics.DrawImage(
   &image,
   destinationRect,
   0, 0,              // upper-left corner of source rectangle
   0.75 * width,      // width of source rectangle
   0.75 * height,     // height of source rectangle
   UnitPixel);
```



На следующем рисунке показан исходный Apple и масштабированный, обрезанный Apple.

![Иллюстрация, показывающая Apple, увеличенная часть исходного Apple](images/cropscale1.png)

 

 



