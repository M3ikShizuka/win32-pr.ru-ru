---
description: Функция D3DXMatrixRotationX (D3DX10Math. h) — строит матрицу, которая поворачивается вокруг оси x.
ms.assetid: 895079bf-b807-4bfd-9222-a7c1251d7d1e
title: Функция D3DXMatrixRotationX (D3DX10Math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXMatrixRotationX
api_type:
- LibDef
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: e338ba63a3c750c2d2b8064113039919b709ed94e282be17f7c042f93a08252d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119990304"
---
# <a name="d3dxmatrixrotationx-function-d3dx10mathh"></a>Функция D3DXMatrixRotationX (D3DX10Math. h)

Строит матрицу, которая поворачивается вокруг оси x.

## <a name="syntax"></a>Синтаксис


```C++
D3DXMATRIX* D3DXMatrixRotationX(
  _Inout_ D3DXMATRIX *pOut,
  _In_    FLOAT      Angle
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тоска* \[ в, out\]
</dt> <dd>

Тип: **[ **D3DXMATRIX**](../direct3d9/d3dxmatrix.md)\***

Указатель на структуру [**D3DXMATRIX**](d3d10-d3dxmatrix.md) , которая является результатом операции.

</dd> <dt>

*Угол* \[ окне\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

Угол поворота в радианах. Углы измеряются по часовой стрелке, если смотреть вдоль оси поворота в направлении начала координат.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **D3DXMATRIX**](../direct3d9/d3dxmatrix.md)\***

Указатель на структуру D3DXMATRIX, повернутую вокруг оси x.

## <a name="remarks"></a>Remarks

Возвращаемое значение для этой функции совпадает со значением, возвращаемым в параметре тоска. Таким образом, функция D3DXMatrixRotationX может использоваться в качестве параметра для другой функции.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10Math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[Математические функции](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 
