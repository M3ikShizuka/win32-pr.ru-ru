---
description: Запрашивает выделение объекта контейнера сетки.
ms.assetid: ec66b393-016b-4572-94dc-5c8903b506a3
title: 'Метод ID3DXAllocateHierarchy:: Креатемешконтаинер (D3dx9anim. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXAllocateHierarchy.CreateMeshContainer
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: fee8b9222358f343b6a8e23435815c8c484a6c8ce86625303e127174d300a197
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120026874"
---
# <a name="id3dxallocatehierarchycreatemeshcontainer-method"></a>Метод ID3DXAllocateHierarchy:: Креатемешконтаинер

Запрашивает выделение объекта контейнера сетки.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CreateMeshContainer(
  [in]                LPCSTR              Name,
  [in]          const D3DXMESHDATA        *pMeshData,
  [in]          const D3DXMATERIAL        *pMaterials,
  [in]          const D3DXEFFECTINSTANCE  *pEffectInstances,
  [in]                DWORD               NumMaterials,
  [in]          const DWORD               *pAdjacency,
  [in]                LPD3DXSKININFO      pSkinInfo,
  [out, retval]       LPD3DXMESHCONTAINER *ppNewMeshContainer
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Имя* \[ окне\]
</dt> <dd>

Тип: **[ **LPCSTR**](../winprog/windows-data-types.md)**

Имя сетки.

</dd> <dt>

*пмешдата* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMESHDATA**](d3dxmeshdata.md) \***

Указатель на структуру данных сетки. См. [**D3DXMESHDATA**](d3dxmeshdata.md).

</dd> <dt>

*пматериалс* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXMATERIAL**](d3dxmaterial.md) \***

Массив материалов, используемых в сетке.

</dd> <dt>

*пеффектинстанцес* \[ окне\]
</dt> <dd>

Тип: **const [**D3DXEFFECTINSTANCE**](d3dxeffectinstance.md) \***

Массив экземпляров эффектов, используемых в сетке. См. [**D3DXEFFECTINSTANCE**](d3dxeffectinstance.md).

</dd> <dt>

*Нумматериалс* \[ окне\]
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

Количество материалов в массиве материалов.

</dd> <dt>

*паджаценци* \[ окне\]
</dt> <dd>

Тип: **const [**DWORD**](../winprog/windows-data-types.md) \***

Массив соседей для сетки.

</dd> <dt>

*пскининфо* \[ окне\]
</dt> <dd>

Тип: **[ **LPD3DXSKININFO**](id3dxskininfo.md)**

Указатель на объект сетки обложки, если обнаружены данные обложки. См. [**ID3DXSkinInfo**](id3dxskininfo.md).

</dd> <dt>

*ппневмешконтаинер* \[ out, retval\]
</dt> <dd>

Тип: **[ **LPD3DXMESHCONTAINER**](d3dxmeshcontainer.md)\***

Возвращает созданный контейнер сетки. См. [**D3DXMESHCONTAINER**](d3dxmeshcontainer.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращаемые значения этого метода реализуются программистом приложения. Как правило, если ошибка не возникает, программа возвращает метод, возвращающий D3D \_ ОК. В противном случае программа возвращает метод, возвращающий соответствующее сообщение об ошибке от D3DERR или D3DXERR, так как это приведет к сбою [**D3DXLoadMeshHierarchyFromX**](d3dxloadmeshhierarchyfromx.md) и возврату ошибки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx9anim. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXAllocateHierarchy](id3dxallocatehierarchy.md)
</dt> </dl>

 

 
