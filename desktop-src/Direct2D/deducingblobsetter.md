---
title: ДедуЦингблобсеттер (D2d1effecthelpers. h)
description: Выводит класс и аргументы, а затем вызывает обратный вызов свойства функции-члена для свойства типа BLOB.
ms.assetid: 4B8B871D-FE5E-4EF3-AEED-A3D92C10E8C6
keywords:
- ДедуЦингблобсеттер Direct2D
topic_type:
- apiref
api_name:
- DeducingBlobSetter
api_location:
- d2d1effecthelpers.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a2d3bbfcc0a48d722bd98456821d7f7df5e8780a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163435"
---
# <a name="deducingblobsetter"></a>дедуЦингблобсеттер

Выводит класс и аргументы, а затем вызывает обратный вызов свойства функции-члена для свойства типа BLOB.

> [!Note]  
> ДедуЦингблобсеттер не следует вызывать напрямую.

 

``` syntax
template<class C, typename I>  
HRESULT DeducingBlobSetter(  
    _In_ HRESULT (C::*callback)(const BYTE *, UINT32),  
    _In_ I *effect,  
    _In_reads_(dataSize) const BYTE *data,  
    UINT32 dataSize,  
    ) 
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D2d1effecthelpers. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Direct2D::D ЕдуЦингблобжеттер**](deducingblobgetter.md)
</dt> </dl>

 

 





