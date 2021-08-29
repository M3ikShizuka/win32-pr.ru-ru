---
description: Функция D3DXGetShaderConstantTableEx — получает таблицу-константу шейдера, внедренную в шейдер.
ms.assetid: f7e846e4-9cb4-4634-95e3-4b2a752978a8
title: Функция D3DXGetShaderConstantTableEx (D3DX9Shader. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXGetShaderConstantTableEx
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 7c3d54a7fa314fe2987d5e1004f7dcd8302753dbb3f0e493d838e3d6407d8db0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120027434"
---
# <a name="d3dxgetshaderconstanttableex-function"></a>Функция D3DXGetShaderConstantTableEx

Возвращает таблицу-константу шейдера, внедренную в шейдер.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DXGetShaderConstantTableEx(
  _In_  const DWORD               *pFunction,
  _In_        DWORD               Flags,
  _Out_       LPD3DXCONSTANTTABLE * ppConstantTable
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пфунктион* \[ окне\]
</dt> <dd>

Тип: **const [**DWORD**](../winprog/windows-data-types.md) \***

Указатель на поток функции DWORD.

</dd> <dt>

*Флаги* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Используйте флаг D3DXCONSTTABLE \_ LARGEADDRESSAWARE, чтобы получить доступ к 4 ГБ виртуального адресного пространства (а не по умолчанию — 2 ГБ). Если дополнительного виртуального адресного пространства не требуется, используйте [**D3DXGetShaderConstantTable**](d3dxgetshaderconstanttable.md).

</dd> <dt>

 *ппконстанттабле* \[ заполняет\]
</dt> <dd>

Тип: **[ **LPD3DXCONSTANTTABLE**](id3dxconstanttable.md)\***

Возвращает интерфейс таблицы констант (см. [**ID3DXConstantTable**](id3dxconstanttable.md)), который управляет таблицей констант.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть одним из следующих: D3DERR \_ инвалидкалл, D3DXERR \_ INVALIDDATA, E \_ OUTOFMEMORY.

## <a name="remarks"></a>Remarks

Таблица констант создается [**D3DXCompileShader**](d3dxcompileshader.md) и внедряется в текст шейдера.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Shader. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>     |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции шейдера](dx9-graphics-reference-d3dx-functions-shader.md)
</dt> </dl>

 

 
