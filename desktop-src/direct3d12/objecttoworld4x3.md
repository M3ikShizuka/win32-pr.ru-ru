---
description: ObjectToWorld4x3 — матрица для преобразования из объектного пространства в мировое пространство.
ms.assetid: ''
title: ObjectToWorld4x3
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ObjectToWorld4x3
api_type:
- NA
ms.openlocfilehash: bc91c6e98aceb13af3f589f873a4b96c2b1843c4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567987"
---
# <a name="objecttoworld4x3"></a>ObjectToWorld4x3

Матрица для преобразования из объектного пространства в мировое пространство. Объектное пространство — это пространство текущей структуры ускорения нижнего уровня.

## <a name="syntax"></a>Синтаксис

```
void ObjectToWorld4x3();

```




## <a name="remarks"></a>Remarks

Матрица является транспоситион матрицы **ObjectToWorld3x4** .

Эту функцию можно вызывать из следующих типов шейдеров райтраЦинг:

* [**Шейдер любых попаданий**](any-hit-shader.md)
* [**Шейдер ближайшего попадания**](closest-hit-shader.md)
* [**Шейдер пересечения**](intersection-shader.md)





## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Справочник по HLSL для трассировки лучей в Direct3D 12](direct3d-12-raytracing-hlsl-reference.md)
</dt> </dl>

 

 




