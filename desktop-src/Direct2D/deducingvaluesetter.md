---
title: ДедуЦингвалуесеттер (D2d1effecthelpers. h)
description: Выводит класс и аргументы, а затем вызывает обратный вызов свойства функции-члена для свойства типа значения.
ms.assetid: 4C3D64A8-0CC0-405A-A5B3-627C2DF25EA1
keywords:
- ДедуЦингвалуесеттер Direct2D
topic_type:
- apiref
api_name:
- DeducingValueSetter
api_location:
- d2d1effecthelpers.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0e002c5a36c8ac0b196dfc5fb25e11f7f9d63806
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163420"
---
# <a name="deducingvaluesetter"></a>дедуЦингвалуесеттер

Выводит класс и аргументы, а затем вызывает обратный вызов свойства функции-члена для свойства типа значения.

> [!Note]  
> ДедуЦингвалуесеттер не следует вызывать напрямую.

 

``` syntax
template<class C, typename P, typename I>
HRESULT DeducingValueSetter(
    _In_ HRESULT (C::*callback)(P),
    _In_ I *effect,
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

[**Direct2D::D ЕдуЦингвалуежеттер**](deducingvaluegetter.md)
</dt> </dl>

 

 





