---
description: Структура D3DXINTERSECTINFO — описывает пересечение лучей-треугольника.
ms.assetid: b6f50fc0-2c8a-4efa-a144-bd0851f8b0ca
title: Структура D3DXINTERSECTINFO (D3dx9mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXINTERSECTINFO
api_type:
- HeaderDef
api_location:
- d3dx9mesh.h
ms.openlocfilehash: f4a63c7f4a479bfbe9dcb49f485ce0acb8db6486
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126969781"
---
# <a name="d3dxintersectinfo-structure"></a>Структура D3DXINTERSECTINFO

Описывает пересечение лучей-треугольника.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXINTERSECTINFO {
  DWORD FaceIndex;
  FLOAT U;
  FLOAT V;
  FLOAT Dist;
} D3DXINTERSECTINFO, *LPD3DXINTERSECTINFO;
```



## <a name="members"></a>Участники

<dl> <dt>

**фацеиндекс**
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

</dd> <dd>

Индекс треугольника, который попадают на луч.

</dd> <dt>

**U**
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

</dd> <dd>

Координата барицентрик в пределах треугольника, на котором пересекается луч.

</dd> <dt>

**V**
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

</dd> <dd>

Координата барицентрик в пределах треугольника, на котором пересекается луч.

</dd> <dt>

**Файле**
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

</dd> <dd>

Расстояние вдоль луча, где произошло пересечение.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Координаты барицентрик определяют точку внутри треугольника с точки зрения вершин треугольника. Более подробное описание координат барицентрик см. в разделе [Описание координат Барицентрик MathWorld](https://mathworld.wolfram.com/BarycentricCoordinates.html).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры D3DX](dx9-graphics-reference-d3dx-structures.md)
</dt> </dl>

 

 
