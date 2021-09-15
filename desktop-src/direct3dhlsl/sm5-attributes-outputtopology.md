---
title: аутпуттопологи
description: Определяет тип выходного примитива для тесселяции.
ms.assetid: 4aba65e5-b005-43fd-a844-c7fbb1b7406c
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 917a927ff80d4abe1b6509fd41281992a998c945
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573642"
---
# <a name="outputtopology"></a>аутпуттопологи

Определяет тип выходного примитива для тесселяции.


```
outputtopology(X)      
```



## <a name="remarks"></a>Комментарии

X должен быть " [**точка**](dx-graphics-hlsl-geometry-shader.md)", " **линия**", " **треугольник \_**" или "треугольник" и должен быть заключен в кавычки. **\_** Ниже приведены допустимые параметры для этого атрибута.


```
[outputtopology("point")]
[outputtopology("line")]
[outputtopology("triangle_cw")]
[outputtopology("triangle_ccw")]
```



Этот атрибут поддерживается в следующих типах шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        | x    |        |          |       |         |



 

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Атрибуты модели шейдеров 5](d3d11-graphics-reference-sm5-attributes.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




