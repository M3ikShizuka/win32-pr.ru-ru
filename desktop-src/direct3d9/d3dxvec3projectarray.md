---
description: Функция D3DXVec3ProjectArray (D3dx9math. h) — проецирует массив (x, y, z, 0) из пространства объекта в пространство экрана.
ms.assetid: cf022741-0bae-4c22-872f-bd94c3721aff
title: Функция D3DXVec3ProjectArray (D3dx9math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXVec3ProjectArray
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 10f0e19ad5bdbff59d7386223c88ed867e8d0d88
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566063"
---
# <a name="d3dxvec3projectarray-function-d3dx9mathh"></a>Функция D3DXVec3ProjectArray (D3dx9math. h)

Проецирует массив (x, y, z, 0) из пространства объекта в пространство экрана.

## <a name="syntax"></a>Синтаксис


```C++
D3DXVECTOR3* D3DXVec3ProjectArray(
  _Inout_       D3DXVECTOR3  *pOut,
  _In_          UINT         OutStride,
  _In_    const D3DXVECTOR3  *pV,
  _In_          UINT         VStride,
  _In_    const D3DVIEWPORT9 *pViewport,
  _In_    const D3DXMATRIX   *pProjection,
  _In_    const D3DXMATRIX   *pView,
  _In_    const D3DXMATRIX   *pWorld,
  _In_          UINT         n
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тоска* \[ в, out\]
</dt> <dd>

Тип: **[ **D3DXVECTOR3**](d3dxvector3.md)\***

Указатель на структуру [**D3DXVECTOR3**](d3dxvector3.md) , которая является результатом операции.

</dd> <dt>

*Шаг* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Шаг между векторами в потоке выходных данных.

</dd> <dt>

*ПС* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](d3dxvector3.md) \***

Указатель на исходную структуру [**D3DXVECTOR3**](d3dxvector3.md) .

</dd> <dt>

*Встриде* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Шаг между векторами во входном потоке данных.

</dd> <dt>

*пвиевпорт* \[ окне\]
</dt> <dd>

Тип: **const [**D3DVIEWPORT9**](d3dviewport9.md) \***

Указатель на структуру [**D3DVIEWPORT9**](d3dviewport9.md) , представляющую окно просмотра.

</dd> <dt>

*ппрожектион* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATRIX**](d3dxmatrix.md) \***

Указатель на структуру [**D3DXMATRIX**](d3dxmatrix.md) , представляющую матрицу проекции.

</dd> <dt>

*pView* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATRIX**](d3dxmatrix.md) \***

Указатель на структуру [**D3DXMATRIX**](d3dxmatrix.md) , представляющую матрицу представления.

</dd> <dt>

*пворлд* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATRIX**](d3dxmatrix.md) \***

Указатель на структуру [**D3DXMATRIX**](d3dxmatrix.md) , представляющую матрицу мира.

</dd> <dt>

*n* \[ в\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Число элементов в массиве.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **D3DXVECTOR3**](d3dxvector3.md)\***

Указатель на структуру [**D3DXVECTOR3**](d3dxvector3.md) , которая представляет собой массив, проецируемый из объектного пространства в пространство экрана.

## <a name="remarks"></a>Remarks

Возвращаемое значение для этой функции совпадает со значением, возвращаемым в параметре *тоска* . Таким образом, функция **D3DXVec3ProjectArray** может использоваться в качестве параметра для другой функции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Математические функции](dx9-graphics-reference-d3dx-functions-math.md)
</dt> <dt>

[**D3DXVec3Unproject**](d3dxvec3unproject.md)
</dt> </dl>

 

 
