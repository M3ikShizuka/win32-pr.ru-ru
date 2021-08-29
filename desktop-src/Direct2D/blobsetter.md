---
title: Блобсеттер (D2d1effecthelpers. h)
description: Вызывает обратный вызов метода задания свойства для функции-члена для свойства типа BLOB.
ms.assetid: 29411D53-1D27-4040-A3C0-B1511E627A32
keywords:
- Блобсеттер Direct2D
topic_type:
- apiref
api_name:
- BlobSetter
api_location:
- d2d1effecthelpers.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b062f32282ee03aabb37f440e3291f71abf3a88963aaecbe0166e5525ad4f661
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119641913"
---
# <a name="blobsetter"></a>блобсеттер

Вызывает обратный вызов метода задания свойства для функции-члена для свойства типа BLOB.

``` syntax
template<typename T, T P, typename I>
HRESULT CALLBACK BlobSetter(
    _In_ IUnknown *effect,
    _In_reads_(dataSize) const BYTE *data,
    UINT32 dataSize  
    ) 
```

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D2d1effecthelpers. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Direct2D:: Блобжеттер**](blobgetter.md)
</dt> </dl>

 

 





