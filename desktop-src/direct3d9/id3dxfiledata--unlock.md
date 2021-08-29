---
description: 'Завершает срок существования указателя Ппдата, возвращенного ID3DXFileData:: Lock.'
ms.assetid: 6032ea1f-3c73-4157-ba3f-41ce9e73d64c
title: 'Метод ID3DXFileData:: Unlock (D3DX9Xof. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXFileData.Unlock
api_type:
- COM
api_location:
- D3dx9.lib
- D3dx9.dll
ms.openlocfilehash: 5eaa1466f722f34bb82152d22c85647cf5afa88310474585b7f944b37af3abf3
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120026234"
---
# <a name="id3dxfiledataunlock-method"></a>Метод ID3DXFileData:: Unlock

Завершает срок существования указателя *ппдата* , возвращенного [**ID3DXFileData:: Lock**](id3dxfiledata--lock.md).

## <a name="syntax"></a>Синтаксис


```C++
BOOL Unlock();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **bool** .](../winprog/windows-data-types.md)**

Возвращаемое значение — S \_ .

## <a name="remarks"></a>Remarks

Необходимо убедиться, что число вызовов [**ID3DXFileData:: Lock**](id3dxfiledata--lock.md) соответствует числу вызовов **ID3DXFileData:: Unlock** . После вызова функции Unlock указатель Ппдата, возвращенный **ID3DXFileData:: Lock** , больше не должен использоваться.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Xof. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>  |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXFileData](id3dxfiledata.md)
</dt> </dl>

 

 
