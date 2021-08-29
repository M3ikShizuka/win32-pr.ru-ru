---
description: Список точек — это коллекция вершин, которые отображаются в виде изолированных точек. Приложение может использовать их в трехмерных сценах для полей звезд или пунктирных линий на поверхности многоугольника.
ms.assetid: 82866b07-5043-433f-974a-0a301d4b5491
title: Списки точек
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f4cf0194c2083c2ebe6bb10741a6fdd41f92d12fface4ed9cbc9478e7a5a8fbc
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119406723"
---
# <a name="point-lists"></a>Списки точек

Список точек — это коллекция вершин, которые отображаются в виде изолированных точек. Приложение может использовать их в трехмерных сценах для полей звезд или пунктирных линий на поверхности многоугольника.

На следующем рисунке показан отрисованный список точек.

![иллюстрация списка точек](images/pointlst.png)

Приложение может применять к списку точек материалы и текстуры. Цвета материала или текстуры отображаются только в нарисованных точках, но не между ними.

Следующий код показывает, как создать вершины для такого списка точек.


```
struct CUSTOMVERTEX
{
    float x,y,z;
};

CUSTOMVERTEX Vertices[] = 
{
    {-5.0, -5.0, 0.0},
    { 0.0,  5.0, 0.0},
    { 5.0, -5.0, 0.0},
    {10.0,  5.0, 0.0},
    {15.0, -5.0, 0.0},
    {20.0,  5.0, 0.0}
};
```



В приведенном ниже примере кода показано, как визуализировать этот список точек в Direct3D 9 с помощью [**IDirect3DDevice9::D равпримитиве**](/windows/win32/api/d3d9helper/nf-d3d9helper-idirect3ddevice9-drawprimitive).


```
//
// It is assumed that d3dDevice is a valid
// pointer to a IDirect3DDevice9 interface.
//
d3dDevice->DrawPrimitive( D3DPT_POINTLIST, 0, 6 );
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Примитивы](primitives.md)
</dt> </dl>

 

 
