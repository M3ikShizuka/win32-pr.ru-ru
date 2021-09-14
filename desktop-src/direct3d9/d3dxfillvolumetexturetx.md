---
description: Функция D3DXFillVolumeTextureTX — использует скомпилированную функцию высокого уровня шейдеров (HLSL) для заполнения каждого шаг текселя каждого уровня mipmap текстуры.
ms.assetid: f082e1d2-c433-482c-9288-58e5c558cdc5
title: Функция D3DXFillVolumeTextureTX (D3dx9tex. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXFillVolumeTextureTX
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 30aac53aa6451885bbd4ae2cac63050b01157974
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066255"
---
# <a name="d3dxfillvolumetexturetx-function"></a>Функция D3DXFillVolumeTextureTX

Использует скомпилированную функцию высокого уровня шейдеров (HLSL) для заполнения каждого шаг текселя каждого уровня mipmap текстуры.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DXFillVolumeTextureTX(
  _In_ LPDIRECT3DVOLUMETEXTURE9 pTexture,
  _In_ LPD3DXTEXTURESHADER      pTextureShader
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*птекстуре* \[ окне\]
</dt> <dd>

Тип: **[ **LPDIRECT3DVOLUMETEXTURE9**](/windows/win32/api/d3d9helper/nn-d3d9helper-idirect3dvolumetexture9)**

Указатель на объект [**IDirect3DVolumeTexture9**](/windows/win32/api/d3d9helper/nn-d3d9helper-idirect3dvolumetexture9) , представляющий заполняемую текстуру.

</dd> <dt>

*птекстурешадер* \[ окне\]
</dt> <dd>

Тип: **[ **LPD3DXTEXTURESHADER**](id3dxtextureshader.md)**

Указатель на объект шейдера текстуры [**ID3DXTextureShader**](id3dxtextureshader.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть одним из следующих: D3DERR \_ NOTAVAILABLE, D3DERR \_ инвалидкалл.

## <a name="remarks"></a>Remarks

Цель текстуры должна быть HLSL функцией, которая имеет следующую семантику:

-   Один входной параметр должен использовать семантику расположения.
-   Один входной параметр должен использовать семантику ПСИЗЕ.
-   Функция должна возвращать параметр, который использует семантику цвета.

Входные параметры могут быть в любом порядке. Пример см. в разделе [ **D3DXFillTextureTX**](d3dxfilltexturetx.md)

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9tex. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>  |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции текстуры в D3DX 9](dx9-graphics-reference-d3dx-functions-texture.md)
</dt> <dt>

[**D3DXFillTextureTX**](d3dxfilltexturetx.md)
</dt> <dt>

[**D3DXFillCubeTextureTX**](d3dxfillcubetexturetx.md)
</dt> </dl>

 

 
