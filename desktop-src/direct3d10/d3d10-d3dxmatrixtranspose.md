---
description: Функция D3DXMatrixTranspose (D3DX10Math. h) — Возвращает матрицу матрицы.
ms.assetid: 934b17cc-39c4-425c-839b-69e080f0efd7
title: Функция D3DXMatrixTranspose (D3DX10Math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXMatrixTranspose
api_type:
- LibDef
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: e20fd8a29ba3f9adec7134a011f8f470c60f7011
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126970057"
---
# <a name="d3dxmatrixtranspose-function-d3dx10mathh"></a>Функция D3DXMatrixTranspose (D3DX10Math. h)

Возвращает матрицу матрицы.

## <a name="syntax"></a>Синтаксис


```C++
D3DXMATRIX* D3DXMatrixTranspose(
  _Inout_       D3DXMATRIX *pOut,
  _In_    const D3DXMATRIX *pM
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тоска* \[ в, out\]
</dt> <dd>

Тип: **[ **D3DXMATRIX**](../direct3d9/d3dxmatrix.md)\***

Указатель на структуру [**D3DXMATRIX**](d3d10-d3dxmatrix.md) , которая является результатом операции.

</dd> <dt>

*PM* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATRIX**](../direct3d9/d3dxmatrix.md) \***

Указатель на исходную структуру D3DXMATRIX.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **D3DXMATRIX**](../direct3d9/d3dxmatrix.md)\***

Указатель на структуру D3DXMATRIX, которая является матрицей матрицы.

## <a name="remarks"></a>Комментарии

Возвращаемое значение для этой функции совпадает со значением, возвращаемым в параметре тоска. Таким образом, функция D3DXMatrixTranspose может использоваться в качестве параметра для другой функции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10Math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Математические функции](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 
