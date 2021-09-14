---
description: Вычитает два вектора 4D.
ms.assetid: 3bc55b38-818e-40eb-859e-495ee28fc4ae
title: Функция D3DXVec4Subtract (D3dx9math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXVec4Subtract
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 1110930d8e37cf04f7de5129c2a72db4ecc4ac8d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126969702"
---
# <a name="d3dxvec4subtract-function"></a>Функция D3DXVec4Subtract

Вычитает два вектора 4D.

## <a name="syntax"></a>Синтаксис


```C++
D3DXVECTOR4* D3DXVec4Subtract(
  _Inout_       D3DXVECTOR4 *pOut,
  _In_    const D3DXVECTOR4 *pV1,
  _In_    const D3DXVECTOR4 *pV2
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тоска* \[ в, out\]
</dt> <dd>

Тип: **[ **D3DXVECTOR4**](d3dxvector4.md)\***

Указатель на структуру [**D3DXVECTOR4**](d3dxvector4.md) , которая является результатом операции.

</dd> <dt>

*pV1* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR4**](d3dxvector4.md) \***

Указатель на исходную структуру [**D3DXVECTOR4**](d3dxvector4.md) .

</dd> <dt>

*pV2* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR4**](d3dxvector4.md) \***

Указатель на исходную структуру [**D3DXVECTOR4**](d3dxvector4.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **D3DXVECTOR4**](d3dxvector4.md)\***

Указатель на структуру [**D3DXVECTOR4**](d3dxvector4.md) , которая является разностью двух векторов.

## <a name="remarks"></a>Комментарии

Возвращаемое значение для этой функции совпадает со значением, возвращаемым в параметре *тоска* . Таким образом, функция **D3DXVec4Subtract** может использоваться в качестве параметра для другой функции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Математические функции](dx9-graphics-reference-d3dx-functions-math.md)
</dt> <dt>

[**D3DXVec3Add**](d3dxvec3add.md)
</dt> <dt>

[**D3DXVec3Scale**](d3dxvec3scale.md)
</dt> </dl>

 

 




