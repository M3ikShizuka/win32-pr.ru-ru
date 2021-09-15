---
description: Задает данные сетки за вычетом данных о положении.
ms.assetid: 30a95ca3-84ab-475d-9654-a3853263056b
title: фвфдата
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d52af6096357c4855d2dc34442c6cd4814b6713b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127565979"
---
# <a name="fvfdata"></a>фвфдата

Задает данные сетки за вычетом данных о положении.

``` syntax
template FVFData
{
    < B6E70A0E-8EF9-4e83-94AD-ECC8B0C04897 >
    DWORD dwFVF;
    DWORD nDWords;
    array DWORD data[nDWords];
} 
```

Где:

-   Двфвф — код ФВФ.
-   Ндвордс — двоичные данные. Число DWORD.
-   \[ндвордс данных \] — массив DWORD, который содержит данные в каждом элементе вершины.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Шаблоны](dx9-graphics-reference-x-file-format-templates.md)
</dt> </dl>

 

 



