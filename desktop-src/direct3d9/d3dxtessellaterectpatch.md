---
description: Разбивает прямоугольное исправление поверхности более высокого порядка в сетку с треугольником.
ms.assetid: d941d994-8a13-49ff-a0b1-b21a3f84ed78
title: Функция D3DXTessellateRectPatch (D3DX9Mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXTessellateRectPatch
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: b7fb3ab1c47ded6fe6ca6548ca6c90b3027e30280acf819d5d024fd0bd554d58
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120119054"
---
# <a name="d3dxtessellaterectpatch-function"></a>Функция D3DXTessellateRectPatch

Разбивает прямоугольное исправление поверхности более высокого порядка в сетку с треугольником.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DXTessellateRectPatch(
  _In_          LPDIRECT3DVERTEXBUFFER9 pVB,
  _In_    const FLOAT                   *pNumSegs,
  _In_    const D3DVERTEXELEMENT9       *pInDecl,
  _In_    const D3DRECTPATCH_INFO       *pRectPatchInfo,
  _Inout_       LPD3DXMESH              pMesh
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ПВБ* \[ окне\]
</dt> <dd>

Тип: **[ **LPDIRECT3DVERTEXBUFFER9**](/windows/win32/api/d3d9helper/nn-d3d9helper-idirect3dvertexbuffer9)**

Буфер вершин, содержащий данные исправления.

</dd> <dt>

*пнумсегс* \[ окне\]
</dt> <dd>

Тип: **const [**float**](../winprog/windows-data-types.md) \***

Указатель на массив из четырех значений с плавающей запятой, определяющих количество сегментов, на которые должны быть разбиты все границы данного обновления прямоугольника при тесселяции. См [**. \_ сведения о D3DRECTPATCH**](d3drectpatch-info.md).

</dd> <dt>

*пиндекл* \[ окне\]
</dt> <dd>

Тип: **const [**D3DVERTEXELEMENT9**](d3dvertexelement9.md) \***

Структура объявления вершин, определяющая данные вершин. См. [**D3DVERTEXELEMENT9**](d3dvertexelement9.md).

</dd> <dt>

*пректпатчинфо* \[ окне\]
</dt> <dd>

Тип: **const [**D3DRECTPATCH \_ info**](d3drectpatch-info.md) \***

Описывает прямоугольное исправление. См [**. \_ сведения о D3DRECTPATCH**](d3drectpatch-info.md).

</dd> <dt>

*пмеш* \[ в, out\]
</dt> <dd>

Тип: **[ **LPD3DXMESH**](id3dxmesh.md)**

Указатель на созданную сетку. См. [**ID3DXMesh**](id3dxmesh.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть одним из следующих: D3DERR \_ инвалидкалл, E \_ OUTOFMEMORY.

## <a name="remarks"></a>Remarks

Используйте [**D3DXRectPatchSize**](d3dxrectpatchsize.md) , чтобы получить количество выходных вершин и индексов, необходимых для функции тесселяции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Mesh. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции сетки](dx9-graphics-reference-d3dx-functions-mesh.md)
</dt> <dt>

[**D3DXTessellateTriPatch**](d3dxtessellatetripatch.md)
</dt> </dl>

 

 
