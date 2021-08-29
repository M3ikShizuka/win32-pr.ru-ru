---
description: Возвращает длину трехмерного вектора.
ms.assetid: 78da506c-3169-48e9-934c-cc09271a10d4
title: Функция D3DXVec3Length (D3dx9math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXVec3Length
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 1ee788ef454f445660228b3e432b5269659916be2c210d7dd1775b7b12f238b9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119122551"
---
# <a name="d3dxvec3length-function"></a>Функция D3DXVec3Length

Возвращает длину трехмерного вектора.

## <a name="syntax"></a>Синтаксис


```C++
FLOAT D3DXVec3Length(
  _In_ const D3DXVECTOR3 *pV
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ПС* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXVECTOR3**](d3dxvector3.md) \***

Указатель на исходную структуру [**D3DXVECTOR3**](d3dxvector3.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **float**](../winprog/windows-data-types.md)**

Длина вектора.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Математические функции](dx9-graphics-reference-d3dx-functions-math.md)
</dt> <dt>

[**D3DXVec3LengthSq**](d3dxvec3lengthsq.md)
</dt> </dl>

 

 
