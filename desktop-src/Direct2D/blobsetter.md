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
ms.openlocfilehash: 2a073db2fb53fa86414ed6081ede0e24c2eb7dcf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164236"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D2d1effecthelpers. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Direct2D:: Блобжеттер**](blobgetter.md)
</dt> </dl>

 

 





