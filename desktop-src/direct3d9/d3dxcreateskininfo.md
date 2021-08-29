---
description: Функция D3DXCreateSkinInfo — создает пустой объект сетки обложки с помощью декларатора.
ms.assetid: c98da2e5-a9eb-4070-8846-b346b5c57fb3
title: Функция D3DXCreateSkinInfo (D3DX9Mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXCreateSkinInfo
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 5d1539e0bf7a552fdb44bb1c2f323af387797a660d4e1bade312000652fb5bbf
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119676144"
---
# <a name="d3dxcreateskininfo-function"></a>Функция D3DXCreateSkinInfo

Создает пустой объект сетки обложки с помощью декларатора.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DXCreateSkinInfo(
  _In_        DWORD             NumVertices,
  _In_  const D3DVERTEXELEMENT9 *pDeclaration,
  _In_        DWORD             NumBones,
  _Out_       LPD3DXSKININFO    *ppSkinInfo
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Нумвертицес* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Число вершин для сетки обложки.

</dd> <dt>

*пдекларатион* \[ окне\]
</dt> <dd>

Тип: **const [**D3DVERTEXELEMENT9**](d3dvertexelement9.md) \***

Массив элементов [**D3DVERTEXELEMENT9**](d3dvertexelement9.md) , описывающих формат вершины для возвращенной сетки.

</dd> <dt>

*Нумбонес* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Число костей для сетки обложки.

</dd> <dt>

*ппскининфо* \[ заполняет\]
</dt> <dd>

Тип: **[ **LPD3DXSKININFO**](id3dxskininfo.md)\***

Адрес указателя на интерфейс [**ID3DXSkinInfo**](id3dxskininfo.md) , представляющий созданный объект сетки обложки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть следующим: E \_ OUTOFMEMORY.

## <a name="remarks"></a>Remarks

Используйте [**сетбонеинфлуенце**](id3dxskininfo--setboneinfluence.md) для заполнения пустого объекта сетки обложки, возвращаемого этим методом.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Mesh. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции сетки](dx9-graphics-reference-d3dx-functions-mesh.md)
</dt> <dt>

[**сетбонеинфлуенце**](id3dxskininfo--setboneinfluence.md)
</dt> </dl>

 

 
