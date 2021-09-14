---
description: Извлекает автоматически сформированный индекс примитива внутри геометрии внутри экземпляра структуры ускорения нижнего уровня.
ms.assetid: ''
title: примитивеиндекс
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PrimitiveIndex
api_type:
- NA
ms.openlocfilehash: d6d1e8ba338a3fb567b583b42074210b514ef360
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066387"
---
# <a name="primitiveindex-function"></a>Функция Примитивеиндекс

Извлекает автоматически сформированный индекс примитива внутри геометрии внутри экземпляра структуры ускорения нижнего уровня.

## <a name="syntax"></a>Синтаксис

```
uint PrimitiveIndex();
```

## <a name="remarks"></a>Remarks

Для **\_ \_ \_ \_ треугольников типа geometry D3D12 райтраЦинг** это индекс треугольника в объекте Geometry.

Для **D3D12 \_ райтраЦинг \_ \_ \_ \_ примитивного \_ типа геометрического объекта ааббс** это индекс в массиве ААББ, определяющем объект Geometry.

Эту функцию можно вызывать из следующих типов шейдеров райтраЦинг:

* [**Шейдер любых попаданий**](any-hit-shader.md)
* [**Шейдер ближайшего попадания**](closest-hit-shader.md)
* [**Шейдер пересечения**](intersection-shader.md)

## <a name="see-also"></a>См. также раздел

* [Справочник по HLSL для трассировки лучей в Direct3D 12](direct3d-12-raytracing-hlsl-reference.md)
