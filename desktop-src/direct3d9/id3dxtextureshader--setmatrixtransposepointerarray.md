---
description: 'Метод ID3DXTextureShader:: Сетматрикстранспосепоинтераррай — задает массив указателей на перекладываемые матрицы.'
ms.assetid: 2b9f1efe-b2ea-416b-a370-202db57b1925
title: 'Метод ID3DXTextureShader:: Сетматрикстранспосепоинтераррай (D3DX9Shader. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXTextureShader.SetMatrixTransposePointerArray
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 46e04c8c86bd0cdf7acea44872d00ad19f620ee6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126888389"
---
# <a name="id3dxtextureshadersetmatrixtransposepointerarray-method"></a>Метод ID3DXTextureShader:: Сетматрикстранспосепоинтераррай

Задает массив указателей на перекладываемые матрицы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMatrixTransposePointerArray(
  [in]       D3DXHANDLE hConstant,
  [in] const D3DXMATRIX **ppMatrix,
  [in]       UINT       Count
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хконстант* \[ окне\]
</dt> <dd>

Тип: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

Уникальный идентификатор массива констант матрицы. См. [D3DXHANDLE](d3dxfx.md).

</dd> <dt>

*ппматрикс* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATRIX**](d3dxmatrix.md) \* \***

Массив указателей на переликвидированные матрицы. См. [**D3DXMATRIX**](d3dxmatrix.md).

</dd> <dt>

*Количество* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Число матриц в массиве.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение D3D \_ ОК. В случае сбоя метода возвращаемое значение может быть D3DERR \_ инвалидкалл.

## <a name="remarks"></a>Комментарии

Переданная матрица содержит основные данные столбца. то есть каждый вектор содержится в столбце.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Shader. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DXTextureShader](id3dxtextureshader.md)
</dt> </dl>

 

 
