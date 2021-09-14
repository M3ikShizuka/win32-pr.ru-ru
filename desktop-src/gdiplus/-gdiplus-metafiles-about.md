---
description: Windows GDI+ предоставляет класс metafile, чтобы можно было записывать и отображать метафайлы.
ms.assetid: a9f9bac4-f3c7-44a1-9f0f-59ff1a27b077
title: Метафайлы (GDI+)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ae75c2185670563f9a9e624d868da5b0e299cbec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065882"
---
# <a name="metafiles-gdi"></a>Метафайлы (GDI+)

Windows GDI+ предоставляет класс [**metafile**](/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-metafile) , чтобы можно было записывать и отображать метафайлы. Метафайл, также называемый векторным изображением, — это изображение, которое хранится в виде последовательности команд и параметров рисования. Команды и параметры, записанные в объекте **Metafile** , могут храниться в памяти или сохраняться в файле или потоке.

GDI+ может отображать метафайлы, сохраненные в следующих форматах:

-   Windows Формат метафайлов (WMF)
-   EMF (Enhanced Metafile —расширенный метафайл)
-   EMF +

GDI+ могут записывать метафайлы в форматах emf и emf +, но не в формате WMF.

emf + — это расширение emf, позволяющее сохранять GDI+ записи. Существует два варианта формата EMF +: EMF + only и EMF + Dual. только метафайлы EMF + содержат только записи GDI+. такие метафайлы могут отображаться GDI+ но не Windows интерфейс графических устройств (GDI). emf + Dual метафайлы содержат записи GDI+ и GDI. каждая запись GDI+ в метафайле emf + Dual сопряжена с альтернативной записью GDI. такие метафайлы могут отображаться GDI+ или GDI.

В следующем примере один параметр и одна команда рисования записываются в файл на диске. Обратите внимание, что в примере создается объект [**Graphics**](/windows/desktop/api/gdiplusgraphics/nl-gdiplusgraphics-graphics) и конструктор объекта **Graphics** получает адрес объекта [**Metafile**](/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-metafile) в качестве аргумента.


```
myMetafile = new Metafile(L"MyDiskFile.emf", hdc);
myGraphics = new Graphics(myMetafile);
   myPen = new Pen(Color(255, 0, 0, 200));
   myGraphics->SetSmoothingMode(SmoothingModeAntiAlias);
   myGraphics->DrawLine(myPen, 0, 0, 60, 40);
delete myGraphics;
delete myPen;
delete myMetafile;
```



Как показано в предыдущем примере, класс [**Graphics**](/windows/desktop/api/gdiplusgraphics/nl-gdiplusgraphics-graphics) является ключом к записи инструкций и параметров в объекте [**Metafile**](/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-metafile) . Любой вызов метода **графического** объекта может быть записан в объект **Metafile** . Аналогичным образом можно задать любое свойство объекта **Graphics** и записать этот параметр в объект **Metafile** . Запись заканчивается, когда объект **Graphics** удаляется или выходит за пределы области.

В следующем примере показан метафайл, созданный в предыдущем примере. Метафайл отображается в левом верхнем углу в (100, 100).


```
Graphics myGraphics(hdc);
Image myImage(L"MyDiskFile.emf");
myGraphics.DrawImage(&myImage, 100, 100);
```



В следующем примере записывается несколько параметров свойств (область отсечения, универсальное преобразование и режим сглаживания) в объекте [**Metafile**](/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-metafile) . Затем код записывает несколько инструкций по рисованию. Инструкции и параметры сохраняются в файле на диске.


```
myMetafile = new Metafile(L"MyDiskFile2.emf", hdc); 
myGraphics = new Graphics(myMetafile);
   myGraphics->SetSmoothingMode(SmoothingModeAntiAlias);
   myGraphics->RotateTransform(30);

   // Create an elliptical clipping region.
   GraphicsPath myPath;
   myPath.AddEllipse(0, 0, 200, 100);
   Region myRegion(&myPath);
   myGraphics->SetClip(&myRegion);

   Pen myPen(Color(255, 0, 0, 255));
   myGraphics->DrawPath(&myPen, &myPath);

   for(INT j = 0; j <= 300; j += 10)
   {
      myGraphics->DrawLine(&myPen, 0, 0, 300 - j, j);
   }
delete myGraphics;
delete myMetafile;
```



В следующем примере отображается изображение метафайла, созданное в предыдущем примере.


```
myGraphics = new Graphics(hdc);
myMetafile = new Metafile(L"MyDiskFile.emf");
myGraphics->DrawImage(myMetafile, 10, 10);
```



На следующем рисунке показаны выходные данные предыдущего кода. Обратите внимание на сглаживание, Область эллиптической обрезки и поворот на 30 градусов.

![снимок экрана окна, содержащего эллипс, заполненный строками, находящимися за пределами эллипса](images/aboutgdip05-art00.png)

 

 



