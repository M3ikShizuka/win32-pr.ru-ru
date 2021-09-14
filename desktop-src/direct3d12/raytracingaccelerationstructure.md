---
title: RaytracingAccelerationStructure
description: Тип ресурса, который может быть объявлен в HLSL и передан в Трацерай для указания ресурса ускорения верхнего уровня, созданного с помощью БуилдрайтраЦингакцелератионструктуре.
ms.assetid: ''
ms.localizationpriority: low
ms.topic: language-reference
ms.date: 05/31/2018
ms.openlocfilehash: beb6f5e397126223e9c0e6959e16a6cca3145517
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066367"
---
# <a name="raytracingaccelerationstructure"></a>RaytracingAccelerationStructure

Тип ресурса, который может быть объявлен в HLSL и передан в [**трацерай**](traceray-function.md) для указания ресурса ускорения верхнего уровня, созданного с помощью **буилдрайтраЦингакцелератионструктуре**. Он привязан как необработанный буфер SRV в таблице дескрипторов или корневом дескрипторе SRV.  Объявление в HLSL выглядит следующим образом:


```
RaytracingAccelerationStructure MyScene[] : register(t3,space1);
```

В этом примере показан массив неограниченного размера структур ускорения, который подразумевает выход из кучи дескрипторов, так как не удается индексировать корневые дескрипторы.

**РайтраЦингакцелератионструктуре** — это непрозрачный ресурс без методов, доступных для шейдеров.


 

 




