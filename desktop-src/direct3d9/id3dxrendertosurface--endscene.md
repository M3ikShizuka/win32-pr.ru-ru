---
description: Завершает сцену.
ms.assetid: f721593e-6cba-4569-8276-6a4ffc0fc37a
title: 'Метод ID3DXRenderToSurface:: Ендсцене (D3dx9core. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXRenderToSurface.EndScene
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: a1671b49250dc76b44078a997a89db6daa5b6e3a7586e53559ebc0b7f2646405
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119790554"
---
# <a name="id3dxrendertosurfaceendscene-method"></a>Метод ID3DXRenderToSurface:: Ендсцене

Завершает сцену.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT EndScene(
  [in] DWORD MipFilter
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Мипфилтер* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Параметры фильтра, перечисленные в [ \_ фильтре D3DX](d3dx-filter.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение D3D \_ ОК. В случае сбоя метода возвращаемое значение может быть одним из следующих: D3DERR \_ инвалидкалл, D3DXERR \_ INVALIDDATA.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9core. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXRenderToSurface](id3dxrendertosurface.md)
</dt> <dt>

[**ID3DXRenderToSurface:: Бегинсцене**](id3dxrendertosurface--beginscene.md)
</dt> </dl>

 

 
