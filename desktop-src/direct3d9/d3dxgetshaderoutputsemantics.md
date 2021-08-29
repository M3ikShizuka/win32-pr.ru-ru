---
description: Получение семантики для всех выходных элементов шейдера.
ms.assetid: 1a3cdd5d-0ea7-48ae-a3f1-030e95b03a42
title: Функция D3DXGetShaderOutputSemantics (D3DX9Shader. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXGetShaderOutputSemantics
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 8fda2c2ac5e331874448e251b14654ba06df33bea6557f75957f8955387b2591
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119986794"
---
# <a name="d3dxgetshaderoutputsemantics-function"></a>Функция D3DXGetShaderOutputSemantics

Получение семантики для всех выходных элементов шейдера.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DXGetShaderOutputSemantics(
  _In_  const DWORD        *pFunction,
  _In_        D3DXSEMANTIC *pSemantics,
  _Out_       UINT         *pCount
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пфунктион* \[ окне\]
</dt> <dd>

Тип: **const [**DWORD**](../winprog/windows-data-types.md) \***

Указатель на поток функции шейдера DWORD.

</dd> <dt>

*псемантикс* \[ окне\]
</dt> <dd>

Тип: **[ **D3DXSEMANTIC**](d3dxsemantic.md)\***

Указатель на массив структур [**D3DXSEMANTIC**](d3dxsemantic.md) . Функция будет заполнять этот массив семантикой для каждого выходного элемента, на который ссылается шейдер. Предполагается, что этот массив содержит по крайней мере элементы MAXD3DDECLLENGTH. Однако вызов **D3DXGetShaderOutputSemantics** с Псемантикс = **null** возвратит количество элементов, необходимых для pCount.

</dd> <dt>

*pCount* \[ заполняет\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)\***

Возвращает количество элементов в Псемантикс.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть одним из следующих: D3DERR \_ инвалидкалл, D3DXERR \_ INVALIDDATA, E \_ OUTOFMEMORY.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Shader. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>     |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции шейдера](dx9-graphics-reference-d3dx-functions-shader.md)
</dt> </dl>

 

 
