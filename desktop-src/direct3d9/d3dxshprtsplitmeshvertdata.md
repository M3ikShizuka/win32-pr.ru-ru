---
description: Структура D3DXSHPRTSPLITMESHVERTDATA
ms.assetid: 8799a680-bf5f-42cc-91aa-1a6aed164ca5
title: Структура D3DXSHPRTSPLITMESHVERTDATA (D3dx9mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXSHPRTSPLITMESHVERTDATA
api_type:
- HeaderDef
api_location:
- d3dx9mesh.h
ms.openlocfilehash: 55424929a3d415fc1b89f7a1af53be849cf90185
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055987"
---
# <a name="d3dxshprtsplitmeshvertdata-structure"></a>Структура D3DXSHPRTSPLITMESHVERTDATA

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXSHPRTSPLITMESHVERTDATA {
  UINT uVertRemap;
  UINT uSubCluster;
  UINT ucVertStatus;
} D3DXSHPRTSPLITMESHVERTDATA, *LPD3DXSHPRTSPLITMESHVERTDATA;
```



## <a name="members"></a>Участники

<dl> <dt>

**увертремап**
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

</dd> <dd>

Вершина в исходной сетке соответствует.

</dd> <dt>

**усубклустер**
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

</dd> <dd>

Индекс кластера относительно кластера.

</dd> <dt>

**уквертстатус**
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

</dd> <dd>

1, если вершина содержит допустимые данные, 0, если это "Full".

</dd> </dl>

## <a name="remarks"></a>Комментарии

Выделено в [**D3DXSHPRTCompSplitMeshSC**](d3dxshprtcompsplitmeshsc.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[Структуры D3DX](dx9-graphics-reference-d3dx-structures.md)
</dt> </dl>

 

 
