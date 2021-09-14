---
description: Windows GDI+ предоставляет функцию жетимажедекодерс, позволяющую определить, какие декодеры изображений доступны на компьютере.
ms.assetid: 793e23de-d959-4feb-8bf6-647a455c85ae
title: Список установленных декодеров
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4a20a4e8ac88fa884483ebeaf6592b8085fde807
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065889"
---
# <a name="listing-installed-decoders"></a>Список установленных декодеров

Windows GDI+ предоставляет функцию [**жетимажедекодерс**](/windows/desktop/api/Gdiplusimagecodec/nf-gdiplusimagecodec-getimagedecoders) , позволяющую определить, какие декодеры изображений доступны на компьютере. **Жетимажедекодерс** возвращает массив объектов [**имажекодеЦинфо**](/windows/win32/api/gdiplusimaging/nl-gdiplusimaging-imagecodecinfo) . Перед вызовом **жетимажедекодерс** необходимо выделить буфер, достаточно большой для получения этого массива. Чтобы определить размер требуемого буфера, можно вызвать [**жетимажедекодерссизе**](/windows/desktop/api/Gdiplusimagecodec/nf-gdiplusimagecodec-getimagedecoderssize) .

В следующем консольном приложении перечислены доступные декодеры изображений:


```
#include <windows.h>
#include <gdiplus.h>
#include <stdio.h>
using namespace Gdiplus;

INT main()
{
   // Initialize GDI+.
   GdiplusStartupInput gdiplusStartupInput;
   ULONG_PTR gdiplusToken;
   GdiplusStartup(&gdiplusToken, &gdiplusStartupInput, NULL);

   UINT  num;        // number of image decoders
   UINT  size;       // size, in bytes, of the image decoder array

   ImageCodecInfo* pImageCodecInfo;

   // How many decoders are there?
   // How big (in bytes) is the array of all ImageCodecInfo objects?
   GetImageDecodersSize(&num, &size);

   // Create a buffer large enough to hold the array of ImageCodecInfo
   // objects that will be returned by GetImageDecoders.
   pImageCodecInfo = (ImageCodecInfo*)(malloc(size));

   // GetImageDecoders creates an array of ImageCodecInfo objects
   // and copies that array into a previously allocated buffer. 
   // The third argument, imageCodecInfo, is a pointer to that buffer. 
   GetImageDecoders(num, size, pImageCodecInfo);

   // Display the graphics file format (MimeType)
   // for each ImageCodecInfo object.
   for(UINT j = 0; j < num; ++j)
   { 
      wprintf(L"%s\n", pImageCodecInfo[j].MimeType);   
   }

   free(pImageCodecInfo);
   GdiplusShutdown(gdiplusToken);
   return 0;
}
```



При запуске предыдущего консольного приложения выходные данные будут выглядеть следующим образом:


```
image/bmp
image/jpeg
image/gif
image/x-emf
image/x-wmf
image/tiff
image/png
image/x-icon
```



 

 
