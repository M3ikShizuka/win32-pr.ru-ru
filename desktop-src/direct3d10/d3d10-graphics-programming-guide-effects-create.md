---
description: Эффект создается путем его загрузки в платформу Effects.
ms.assetid: b0a12620-4f8f-44d9-bc73-2c3ab30f80af
title: Создание влияния (Direct3D 10)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 75014688c62e6f8f0463c430b0b17aafd28e0ad3764d00b8a357a6613565d87d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119567064"
---
# <a name="create-an-effect-direct3d-10"></a>Создание влияния (Direct3D 10)

Эффект создается путем его загрузки в платформу Effects. Если результат не был скомпилирован, он будет скомпилирован при создании. Эффекты, которые уже загружены в память, можно создать путем вызова [**D3DX10CreateEffectFromMemory**](d3dx10createeffectfrommemory.md). В следующем примере кода используется [**D3DX10CreateEffectFromFile**](d3dx10createeffectfromfile.md) для создания эффектов из файла.


```
ID3D10Effect* g_pEffect10 = NULL; 

// Read the effect file 
D3DX10CreateEffectFromFile( "BasicHLSL10.fx", NULL, NULL,
  D3D10_SHADER_ENABLE_STRICTNESS, 0, pd3dDevice, NULL, NULL, 
  &g_pEffect10, NULL );
```



Для чтения результата требуются те же параметры, что и при компиляции влияния, а также устройство и пул.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Отрисовка влияния (Direct3D 10)](d3d10-graphics-programming-guide-effects-render.md)
</dt> </dl>

 

 



