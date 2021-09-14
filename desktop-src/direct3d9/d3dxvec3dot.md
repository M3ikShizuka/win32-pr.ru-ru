---
description: Определяет скалярное произведение двух трехмерных векторов.
ms.assetid: 61aa7751-cc06-4673-929b-d7c1e691e395
title: Функция D3DXVec3Dot (D3dx9math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXVec3Dot
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 22d6930a44f129154482f9b1aab24337e8bcdc83
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127052933"
---
# <a name="d3dxvec3dot-function"></a>Функция D3DXVec3Dot

Определяет скалярное произведение двух трехмерных векторов.

## <a name="syntax"></a>Синтаксис


```C++
FLOAT D3DXVec3Dot(
  _In_ const D3DXVECTOR3 *pV1,
  _In_ const D3DXVECTOR3 *pV2
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pV1* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](d3dxvector3.md) \***

Указатель на исходную структуру [**D3DXVECTOR3**](d3dxvector3.md) .

</dd> <dt>

*pV2* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](d3dxvector3.md) \***

Указатель на исходную структуру [**D3DXVECTOR3**](d3dxvector3.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **float**](../winprog/windows-data-types.md)**

Точка-произведение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Математические функции](dx9-graphics-reference-d3dx-functions-math.md)
</dt> <dt>

[**D3DXVec3Cross**](d3dxvec3cross.md)
</dt> </dl>

 

 
