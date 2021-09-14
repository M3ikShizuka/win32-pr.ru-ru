---
description: Функция D3DXIntersectTri (D3DX10math. h) — вычисление пересечения луча и треугольника.
ms.assetid: 819f2543-8046-47c9-93b8-7d888264786f
title: Функция D3DXIntersectTri (D3DX10math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXIntersectTri
api_type:
- LibDef
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: c8bf502cca48701a7d71a083e515f9988cafe303
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241639"
---
# <a name="d3dxintersecttri-function-d3dx10mathh"></a>Функция D3DXIntersectTri (D3DX10math. h)

Вычисление пересечения луча и треугольника.

## <a name="syntax"></a>Синтаксис


```C++
BOOL D3DXIntersectTri(
  _In_  const D3DXVECTOR3 *p0,
  _In_  const D3DXVECTOR3 *p1,
  _In_  const D3DXVECTOR3 *p2,
  _In_  const D3DXVECTOR3 *pRayPos,
  _In_  const D3DXVECTOR3 *pRayDir,
  _Out_       FLOAT       *pU,
  _Out_       FLOAT       *pV,
  _Out_       FLOAT       *pDist
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*P0* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](../direct3d9/d3dxvector3.md) \***

Указатель на структуру [**D3DXVECTOR3**](d3d10-d3dxvector3.md) , описывающий первую точку вершинного треугольника.

</dd> <dt>

*P1* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](../direct3d9/d3dxvector3.md) \***

Указатель на структуру [**D3DXVECTOR3**](d3d10-d3dxvector3.md) , описывающий вторую точку вершинного треугольника.

</dd> <dt>

*P2* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](../direct3d9/d3dxvector3.md) \***

Указатель на структуру [**D3DXVECTOR3**](d3d10-d3dxvector3.md) , описывающий третье расположение вершины треугольника.

</dd> <dt>

*прайпос* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](../direct3d9/d3dxvector3.md) \***

Указатель на структуру [**D3DXVECTOR3**](d3d10-d3dxvector3.md) , указывающий точку, с которой начинается луч.

</dd> <dt>

*прайдир* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](../direct3d9/d3dxvector3.md) \***

Указатель на структуру [**D3DXVECTOR3**](d3d10-d3dxvector3.md) , в которой указывается направление луча.

</dd> <dt>

*PU* \[ заполняет\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)\***

Барицентрик координаты нажатия, U.

</dd> <dt>

*ПС* \[ заполняет\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)\***

Барицентрик координаты точки останова, V.

</dd> <dt>

*пдист* \[ заполняет\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)\***

Расстояние для параметра пересечения лучей.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **bool** .](../winprog/windows-data-types.md)**

Возвращает **значение true** , если луч пересекает область треугольника. В противном случае возвращает **значение false**.

## <a name="remarks"></a>Remarks

Любая точка в плоскости V1V2V3 может быть представлена координатой барицентрик (U, V). Параметр U управляет тем, сколько v2 имеет взвешенное значение в результате, а параметр V определяет, сколько будет иметь взвешенное значение v3 в результате. Наконец, значение \[ 1 (U + V) \] определяет, сколько единиц измерения v1 будет взвешено по результату.

Координаты барицентрик — это форма общих координат. В этом контексте использование координат барицентрик представляет собой изменение в системах координат. Что содержит значение true для декартовых координат, имеет значение true для координат барицентрик.

Координаты барицентрик определяют точку внутри треугольника с точки зрения вершин треугольника. Более подробное описание координат барицентрик см. в разделе [Описание координат Барицентрик MathWorld](https://mathworld.wolfram.com/BarycentricCoordinates.html).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции сетки](d3d10-graphics-reference-d3dx10-functions-mesh.md)
</dt> </dl>

 

 
