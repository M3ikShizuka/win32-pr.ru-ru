---
description: Возвращает количество вершин, на которые влияет заданная кость.
ms.assetid: e92361ea-4269-4d63-a8d1-560a486b6563
title: 'Метод ID3DX10SkinInfo:: Жетбонеинфлуенцекаунт (D3DX10. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DX10SkinInfo.GetBoneInfluenceCount
api_type:
- COM
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: baea07c840210a785e7bf54ad14bb4f6102e8ad2212c5845e52c3c6257439e51
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119634284"
---
# <a name="id3dx10skininfogetboneinfluencecount-method"></a>Метод ID3DX10SkinInfo:: Жетбонеинфлуенцекаунт

Возвращает количество вершин, на которые влияет заданная кость.

## <a name="syntax"></a>Синтаксис


```C++
UINT GetBoneInfluenceCount(
  [in] UINT BoneIndex
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Бонеиндекс* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Индекс, указывающий существующую кость. Значение должно находиться в диапазоне от 0 до значения, возвращаемого [**ID3DX10SkinInfo:: жетнумбонес**](id3dx10skininfo-getnumbones.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Если метод выполнен успешно, возвращается значение S \_ . Если метод завершается со сбоем, возвращаемое значение может быть следующим: E \_ INVALIDARG.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DX10SkinInfo](id3dx10skininfo.md)
</dt> <dt>

[Интерфейсы D3DX](d3d10-graphics-reference-d3dx10-interfaces.md)
</dt> </dl>

 

 
