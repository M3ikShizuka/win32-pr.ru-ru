---
title: instance
description: Используйте этот атрибут для экземпляра шейдера Geometry.
ms.assetid: 0e487e52-53d0-4193-99b2-fd018a061b42
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 4749e11db00b38e5e223e11315de86656b2f6488
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127263888"
---
# <a name="instance"></a>instance

Используйте этот атрибут для экземпляра шейдера Geometry.


```
instance(X)   
```



## <a name="remarks"></a>Remarks

X — это целочисленный индекс, указывающий количество экземпляров, которые должны быть выполнены для каждого рисуемого элемента (например, для каждого треугольника). При использовании этого атрибута используйте [SV \_ гсинстанцеид](sv-gsinstanceid.md) , чтобы указать, какой экземпляр шейдера Geometry выполняется.

Этот атрибут поддерживается в следующих типах шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        | x        |       |         |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Атрибуты модели шейдеров 5](d3d11-graphics-reference-sm5-attributes.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




