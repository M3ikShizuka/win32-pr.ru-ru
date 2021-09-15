---
title: макстессфактор
description: Указывает максимальное значение, которое будет возвращаться шейдером поверхности для любого фактора тесселяции.
ms.assetid: 2c12ed56-cd64-4143-8dda-6998aa212356
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 261ab17bd40c24c19b4b929f2e8307ccc6bb9b56
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573643"
---
# <a name="maxtessfactor"></a>макстессфактор

Указывает максимальное значение, которое будет возвращаться шейдером поверхности для любого фактора тесселяции.


```
maxtessfactor(X)   
```



## <a name="remarks"></a>Комментарии

Этот атрибут помещает верхнюю границу объема запрошенной тесселяции, чтобы помочь драйверу определить максимальный объем ресурсов, необходимых для тесселяции.

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

 

 




