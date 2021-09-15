---
description: Построитель текстуры, который вызывается, когда он включен, и было определено ближайшее попадание или закончено поиск пересечения лучей.
ms.assetid: ''
title: Шейдер ближайшего попадания
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- RAY_FLAG
api_type:
- NA
ms.openlocfilehash: 347ad66dce0a81b929d5dc3c82051bf84226e723
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570914"
---
# <a name="closest-hit-shader"></a>Шейдер ближайшего попадания

Построитель текстуры, который вызывается, когда он включен, и было определено ближайшее попадание или закончено поиск пересечения лучей. В этом шейдере, как правило, происходит заливка поверхности и дополнительное поколение лучей.  Ближайшие шейдеры попадания должны объявлять параметр полезной нагрузки, за которым следует параметр attributes.  Каждый должен быть определяемым пользователем типом структуры, соответствующим типам, используемым для [**трацерай**](traceray-function.md) и [**репорсит**](reporthit-function.md) соответственно, или [**структурой атрибутов пересечения**](intersection-attributes.md) при использовании пересечения треугольника с фиксированной функцией.

## <a name="shader-type-attribute"></a>Атрибут типа шейдера


```
[shader("closesthit")]
```



## <a name="example"></a>Пример

```
[shader("closesthit")]
void closesthit_main(inout MyPayload payload, in MyAttributes attr)
{
    CallShader( ... );  // maybe
    // update payload for surface
    // trace reflection
    float3 worldRayOrigin = WorldRayOrigin() + WorldRayDirection() * RayTCurrent();
    float3 worldNormal = mul(attr.normal, (float3x3)ObjectToWorld3x4());
    RayDesc reflectedRay = { worldRayOrigin, SceneConstants.Epsilon,
                             ReflectRay(WorldRayDirection(), worldNormal),
                             SceneConstants.TMax };
    TraceRay(MyAccelerationStructure,
             SceneConstants.RayFlags,
             SceneConstants.InstanceInclusionMask,
             SceneConstants.RayContributionToHitGroupIndex,
             SceneConstants.MultiplierForGeometryContributionToHitGroupIndex,
             SceneConstants.MissShaderIndex,
             reflectedRay,
             payload);
    // Combine final contributions into ray payload
    // this ray query is now complete.
    // Alternately, could look at data in payload result based on that make other TraceRay
    // calls.  No constraints on the code structure.
}

```

 

 




