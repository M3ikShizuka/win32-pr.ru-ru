---
title: P (OpenGL)
description: Определения терминов OpenGL, которые начинаются с буквы P.
ROBOTS: NOINDEX, NOFOLLOW
ms.assetid: bc7b0c93-af06-44a4-8bb8-adc0c6fedb6e
keywords:
- parameters
- подразделение перспективы
- пиксели
- точки
- многоугольники
- Primitives
- матрицы проекции
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 213fd30866deeaacec6408752424444190801164a3f15de2417fbd308f3beb6b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118936395"
---
# <a name="p-opengl"></a>P (OpenGL)

[A](a.md) [B](b.md) [C](c.md) [D](d.md) [E](e.md) [F](f.md) [G](g.md) [р.](h.md) [](i.md) [J K](jk.md) [L](l.md) [M](m.md) [N](n.md) [O](o.md) P [Q](q.md) [R](r.md) [S](s.md) [T](t.md) [U V](u-v.md) [W](w.md) [X Y Z](x-y-z.md)

<dl> <dt>

<span id="opengl_parameter"></span><span id="OPENGL_PARAMETER"></span>**параметр**
</dt> <dd>

Значение, передаваемое в качестве аргумента команде OpenGL. Иногда одно из значений, передаваемых по ссылке на команду OpenGL.

</dd> <dt>

<span id="opengl_perspective_division"></span><span id="OPENGL_PERSPECTIVE_DIVISION"></span>**подразделение перспективы**
</dt> <dd>

Деление x, y и z на w выполняется в координатах обрезки. См. также [координаты клипов](c.md).

</dd> <dt>

<span id="opengl_pixel"></span><span id="OPENGL_PIXEL"></span>**растров**
</dt> <dd>

Элемент Picture. Биты в расположении (x, y) всех битпланес в буфера кадров составляют один пиксель (x, y). В изображении в памяти клиента пиксель — это одна группа элементов. В координатах окна OpenGL каждый пиксель соответствует области экрана 1,0 x 1.0. Координаты левого нижнего угла в именах пикселей x, y — (x, y), а правый верхний угол — (x + 1, y + 1).

</dd> <dt>

<span id="opengl_point"></span><span id="OPENGL_POINT"></span>**точки**
</dt> <dd>

Точное расположение в пространстве, которое подготавливается к просмотру как точка конечного диаметра.

</dd> <dt>

<span id="opengl_polygon"></span><span id="OPENGL_POLYGON"></span>**фигуры**
</dt> <dd>

Близкое к краю поверхность, ограниченная краями, заданным вершинами. Каждый треугольник сетки треугольника — это многоугольник, как и каждый грани четырехсторонней сетки грани четырехсторонней. Прямоугольник, заданный параметром Глрект, также является многоугольником.

</dd> <dt>

<span id="opengl_primitive"></span><span id="OPENGL_PRIMITIVE"></span>**простого**
</dt> <dd>

Фигура (точка, линия, многоугольник, точечный рисунок или изображение), которую можно изобразить, сохранять и манипулировать как дискретными сущностями; элементы, из которых создаются крупные графические модели.

</dd> <dt>

<span id="opengl_projection_matrix"></span><span id="OPENGL_PROJECTION_MATRIX"></span>**матрица проекции**
</dt> <dd>

Матрица 4x4, которая преобразует точки, линии, многоугольники и растровые позиции из координат глаз в координаты отсечения.

</dd> </dl>

 

 




