---
description: Windows GDI+ предоставляет плоский API, состоящий из примерно 600 функций. Эти плоские функции API упаковываются классом SolidBrush C++.
ms.assetid: b427b8ab-66fd-4f57-b08e-5f337a9ac9af
title: Функции SolidBrush
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: dc9feb2676c60b3f504315f75303aadb16a1cd1f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461092"
---
# <a name="solidbrush-functions"></a>Функции SolidBrush

Windows GDI+ предоставляет плоский API, который состоит из примерно 600 функций, реализованных в Gdiplus.dll и объявленных в гдиплусфлат. h. функции в GDI+ плоском API упаковываются в коллекцию из примерно 40 классов C++. Не рекомендуется вызывать функции непосредственно в неструктурированном API. при вызове GDI+ рекомендуется сделать это, вызвав методы и функции, предоставляемые оболочками C++. Служба технической поддержки Майкрософт не предоставит поддержку для кода, который напрямую вызывает плоский API. дополнительные сведения об использовании этих методов-оболочек см. в разделе [GDI+ плоский API](-gdiplus-flatapi-flat.md).

Следующие плоские функции API упаковываются классом [**SolidBrush**](/windows/desktop/api/gdiplusbrush/nl-gdiplusbrush-solidbrush) C++.

## <a name="brush-functions-and-corresponding-wrapper-methods"></a>Функции-кисти и соответствующие методы-оболочки



| Плоская функция                                                                               | Метод-оболочка                                                                                       | Remarks                                                                                 |
|---------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| **Гпстатус ВИНГДИПАПИ Гдипкреатесолидфилл (цвет ARGB, \* \* кисть гпсолидфилл)**<br/>   | [**SolidBrush:: SolidBrush (в цветовой& константы)**](/windows/win32/api/gdiplusbrush/nf-gdiplusbrush-solidbrush-solidbrush(constsolidbrush_)) | Создает объект [**SolidBrush**](/windows/desktop/api/gdiplusbrush/nl-gdiplusbrush-solidbrush) на основе цвета |
| **Гпстатус ВИНГДИПАПИ Гдипсетсолидфиллколор ( \* кисть гпсолидфилл, цвет ARGB)**<br/>   | [**SolidBrush:: Сетколор (в цветах констант& Color)**](/windows/desktop/api/Gdiplusbrush/nf-gdiplusbrush-solidbrush-setcolor)     | Задает цвет сплошной кисти                                                      |
| **Гпстатус ВИНГДИПАПИ Гдипжетсолидфиллколор ( \* кисть гпсолидфилл, \* цвет ARGB)**<br/> | [**SolidBrush::-Color (цвет OUT \* ) const**](/windows/desktop/api/Gdiplusbrush/nf-gdiplusbrush-solidbrush-getcolor)   | Возвращает цвет сплошной кисти                                                      |



 

 

 
