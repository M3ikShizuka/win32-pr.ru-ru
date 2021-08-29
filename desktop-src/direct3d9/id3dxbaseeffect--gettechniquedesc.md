---
description: Возвращает описание метода.
ms.assetid: 12122858-1e54-446c-8f12-20cc62499d74
title: 'Метод ID3DXBaseEffect:: Жеттечникуедеск (D3DX9Effect. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXBaseEffect.GetTechniqueDesc
api_type:
- COM
api_location:
- D3dx9.lib
- D3dx9.dll
ms.openlocfilehash: e7d2d317e49c1f883cf7b509eeeb59d435c6df29fcf213f06d0daf8999382cf7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119848634"
---
# <a name="id3dxbaseeffectgettechniquedesc-method"></a>Метод ID3DXBaseEffect:: Жеттечникуедеск

Возвращает описание метода.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetTechniqueDesc(
  [in]  D3DXHANDLE         hTechnique,
  [out] D3DXTECHNIQUE_DESC *pDesc
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хтечникуе* \[ окне\]
</dt> <dd>

Тип: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

Обрабатывающий метод. См. раздел [Handles (Direct3D 9)](handles.md).

</dd> <dt>

*пдеск* \[ заполняет\]
</dt> <dd>

Тип: **[ **D3DXTECHNIQUE \_ DESC**](d3dxtechnique-desc.md)\***

Возвращает описание метода. См. [**D3DXTECHNIQUE \_ DESC**](d3dxtechnique-desc.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение S \_ . В случае сбоя метода возвращаемое значение может быть D3DERR \_ инвалидкалл.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Effect. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DXBaseEffect](id3dxbaseeffect.md)
</dt> </dl>

 

 




