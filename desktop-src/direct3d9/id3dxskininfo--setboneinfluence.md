---
description: Задает значение влияния для кости.
ms.assetid: c6dc8a33-8f5c-47d0-8637-a2492b1e3089
title: 'Метод ID3DXSkinInfo:: Сетбонеинфлуенце (D3DX9Mesh. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXSkinInfo.SetBoneInfluence
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 7c34dc8f3d813afbc4ab5be4955f2c373c7af20e752acde1fa84f1a23b5fa2b2
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119893264"
---
# <a name="id3dxskininfosetboneinfluence-method"></a>Метод ID3DXSkinInfo:: Сетбонеинфлуенце

Задает значение влияния для кости.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetBoneInfluence(
  [in]       DWORD Bone,
  [in]       DWORD numInfluences,
  [in] const DWORD *vertices,
  [in] const FLOAT *weights
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Кость* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Номер кости.

</dd> <dt>

*нуминфлуенцес* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Количество повлияет на.

</dd> <dt>

*вершины* \[ окне\]
</dt> <dd>

Тип: **const [**DWORD**](../winprog/windows-data-types.md) \***

Массив вершин, на которые влияет кость.

</dd> <dt>

*весовые коэффициенты* \[ окне\]
</dt> <dd>

Тип: **const [**float**](../winprog/windows-data-types.md) \***

Массив весов, на которые влияет кость.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение D3D \_ ОК. В случае сбоя метода возвращаемое значение может быть D3DERR \_ инвалидкалл.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Mesh. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXSkinInfo](id3dxskininfo.md)
</dt> <dt>

[**ID3DXSkinInfo:: Жетбонеинфлуенце**](id3dxskininfo--getboneinfluence.md)
</dt> <dt>

[**ID3DXSkinInfo:: Жетнумбонеинфлуенцес**](id3dxskininfo--getnumboneinfluences.md)
</dt> </dl>

 

 
