---
description: после внесения незначительных изменений в код можно отправить Windows GDI+ вывода на принтер, а не на экран.
ms.assetid: be6286e9-d125-40ad-b33e-b4e734ac2709
title: Печать (GDI+)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8e3b60010bcb63c553a96c5d70826f3fe0d3d4aa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055674"
---
# <a name="printing-gdi"></a>Печать (GDI+)

после внесения незначительных изменений в код можно отправить Windows GDI+ вывода на принтер, а не на экран. Чтобы рисовать на принтере, получите маркер контекста устройства для принтера и передайте этот обработчик [**графическому**](/windows/desktop/api/gdiplusgraphics/nl-gdiplusgraphics-graphics) конструктору. размещайте GDI+ команды рисования между вызовами [стартдок](/windows/win32/api/wingdi/nf-wingdi-startdocw) и [енддок](/windows/win32/api/wingdi/nf-wingdi-enddoc).

в следующих разделах рассматриваются более подробные сведения об отправке GDI+ вывода на принтеры.

-   [Отправка выходных данных GDI+ на принтер](-gdiplus-sending-gdi-output-to-a-printer-use.md)
-   [Отображение диалогового окна «Печать»](-gdiplus-displaying-a-print-dialog-box-use.md)
-   [Оптимизация печати через дескриптор принтера](-gdiplus-optimizing-printing-by-providing-a-printer-handle-use.md)

 

 



