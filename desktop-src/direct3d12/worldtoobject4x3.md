---
description: WorldToObject4x3 — матрица для преобразования из мирового пространства в объектно-пространство.
ms.assetid: ''
title: WorldToObject4x3
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WorldToObject4x3
api_type:
- NA
ms.openlocfilehash: 334a79352345fb35fbbafe68248a221bdaab9f6d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145569"
---
# <a name="worldtoobject4x3"></a>WorldToObject4x3

Матрица для преобразования из мирового пространства в объектно-пространство. Объектное пространство — это пространство текущей структуры ускорения нижнего уровня.

## <a name="syntax"></a>Синтаксис

```
void WorldToObject4x3();

```




## <a name="remarks"></a>Remarks

Матрица является транспоситион матрицы **WorldToObject3x4** .

Эту функцию можно вызывать из следующих типов шейдеров райтраЦинг:

* [**Шейдер любых попаданий**](any-hit-shader.md)
* [**Шейдер ближайшего попадания**](closest-hit-shader.md)
* [**Шейдер пересечения**](intersection-shader.md)





## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Справочник по HLSL для трассировки лучей в Direct3D 12](direct3d-12-raytracing-hlsl-reference.md)
</dt> </dl>

 

 




