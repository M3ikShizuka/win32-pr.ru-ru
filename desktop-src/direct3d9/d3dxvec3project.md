---
description: Функция D3DXVec3Project (D3dx9math. h) — проецирует трехмерный вектор из объектного пространства в пространство экрана.
ms.assetid: b012771d-052f-4bf9-b39c-387d8a63fa59
title: Функция D3DXVec3Project (D3dx9math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXVec3Project
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: a5a9abcb54c883d74bde831570b9df0b40fedfae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127052929"
---
# <a name="d3dxvec3project-function-d3dx9mathh"></a>Функция D3DXVec3Project (D3dx9math. h)

Проецирует трехмерный вектор из объектного пространства в пространство экрана.

## <a name="syntax"></a>Синтаксис


```C++
D3DXVECTOR3* D3DXVec3Project(
  _Inout_       D3DXVECTOR3  *pOut,
  _In_    const D3DXVECTOR3  *pV,
  _In_    const D3DVIEWPORT9 *pViewport,
  _In_    const D3DXMATRIX   *pProjection,
  _In_    const D3DXMATRIX   *pView,
  _In_    const D3DXMATRIX   *pWorld
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тоска* \[ в, out\]
</dt> <dd>

Тип: **[ **D3DXVECTOR3**](d3dxvector3.md)\***

Указатель на структуру [**D3DXVECTOR3**](d3dxvector3.md) , которая является результатом операции.

</dd> <dt>

*ПС* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](d3dxvector3.md) \***

Указатель на исходную структуру [**D3DXVECTOR3**](d3dxvector3.md) .

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

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **D3DXVECTOR3**](d3dxvector3.md)\***

Указатель на структуру [**D3DXVECTOR3**](d3dxvector3.md) , которая является вектором, проецируемым из пространства объекта в пространство экрана.

## <a name="remarks"></a>Комментарии

Возвращаемое значение для этой функции совпадает со значением, возвращаемым в параметре *тоска* . Таким образом, функция **D3DXVec3Project** может использоваться в качестве параметра для другой функции.

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

 

 




