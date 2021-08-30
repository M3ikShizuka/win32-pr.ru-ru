---
description: Возвращает сведения о материалах, сохраненные в файлах Direct3D (. x).
ms.assetid: dfa021ba-61d8-4f99-9bbb-0cfbe11b787d
title: Структура D3DXMATERIAL (D3dx9mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXMATERIAL
api_type:
- HeaderDef
api_location:
- d3dx9mesh.h
ms.openlocfilehash: c90b03f5d6526fc3545ff1ffe1d48dfea20f96ea4ae34602f885ce7f062003b6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120027414"
---
# <a name="d3dxmaterial-structure"></a>Структура D3DXMATERIAL

Возвращает сведения о материалах, сохраненные в файлах Direct3D (. x).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXMATERIAL {
  D3DMATERIAL9 MatD3D;
  LPSTR        pTextureFilename;
} D3DXMATERIAL, *LPD3DXMATERIAL;
```



## <a name="members"></a>Члены

<dl> <dt>

**MatD3D**
</dt> <dd>

Тип: **[ **D3DMATERIAL9**](d3dmaterial9.md)**

</dd> <dd>

Структура [**D3DMATERIAL9**](d3dmaterial9.md) , описывающая свойства материала.

</dd> <dt>

**птекстурефиленаме**
</dt> <dd>

Тип: **LPSTR**

</dd> <dd>

Указатель на строку, указывающую имя файла текстуры.

</dd> </dl>

## <a name="remarks"></a>Remarks

Функции [**D3DXLoadMeshFromX**](d3dxloadmeshfromx.md) и [**D3DXLoadMeshFromXof**](d3dxloadmeshfromxof.md) возвращают массив структур **D3DXMATERIAL** , которые определяют цвет материала и название текстуры для каждого материала в сети. Затем приложение требуется для загрузки текстуры.

Тип LPD3DXMATERIAL определяется как указатель на структуру **D3DXMATERIAL** .


```
typedef struct D3DXMATERIAL* LPD3DXMATERIAL;
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Структуры D3DX](dx9-graphics-reference-d3dx-structures.md)
</dt> <dt>

[**D3DXLoadMeshFromX**](d3dxloadmeshfromx.md)
</dt> <dt>

[**D3DXLoadMeshFromXof**](d3dxloadmeshfromxof.md)
</dt> </dl>

 

 




