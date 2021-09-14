---
title: ДедуЦингблобжеттер (D2d1effecthelpers. h)
description: Выводит класс и аргументы, а затем вызывает обратный вызов метода получения свойства функции-члена для свойства типа BLOB.
ms.assetid: 1B8800CB-2AD0-4684-99D7-986F6C53A6F1
keywords:
- ДедуЦингблобжеттер Direct2D
topic_type:
- apiref
api_name:
- DeducingBlobGetter
api_location:
- d2d1effecthelpers.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5f7ca5cc37a9fbd79807e258a87a199be7319ce3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163439"
---
# <a name="deducingblobgetter"></a>дедуЦингблобжеттер

Выводит класс и аргументы, а затем вызывает обратный вызов метода получения свойства функции-члена для свойства типа BLOB.

> [!Note]  
> ДедуЦингблобжеттер не следует вызывать напрямую.

 

``` syntax
template<class C, typename I>  
HRESULT DeducingBlobGetter(  
    _In_ HRESULT (C::*callback)(BYTE *, UINT32, UINT32*) const,  
    _In_ const I *effect,  
    _Out_writes_opt_(dataSize) BYTE *data,  
    UINT32 dataSize,  
    _Out_opt_ UINT32 *actualSize  
    ) 
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D2d1effecthelpers. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Direct2D::D ЕдуЦингблобсеттер**](deducingblobsetter.md)
</dt> </dl>

 

 





