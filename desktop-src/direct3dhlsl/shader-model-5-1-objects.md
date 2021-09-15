---
title: Объекты модели шейдеров 5,1
description: В модель шейдера 5,1 добавлены следующие объекты.
ms.assetid: 2958618D-54C6-4860-9910-B45AAB73CCFD
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 376ce272e789501e21f5866be37f56daf31bc829
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573663"
---
# <a name="shader-model-51-objects"></a>Объекты модели шейдеров 5,1

В модель шейдера 5,1 добавлены следующие объекты.

Для [представлений порядка средства прорисовки](/windows/desktop/direct3d11/rasterizer-order-views) (доступно в D3D 11.3 и D3D12) следующие объекты являются новыми и разрешаются только в шейдере пикселей. Обратите внимание, что поддерживаемые методы идентичны соответствующим объектам UAV.



| Объект средства программной прорисовки                                   | Объект UAV                                                              |
|------------------------------------|---------------------------------------------------------------|
| растеризерордередбуффер            | [**рвбуффер**](sm5-object-rwbuffer.md)                       |
| растеризерордередбитеаддрессбуффер | [**рвбитеаддрессбуффер**](sm5-object-rwbyteaddressbuffer.md) |
| растеризерордередструктуредбуффер  | [**рвструктуредбуффер**](sm5-object-rwstructuredbuffer.md)   |
| RasterizerOrderedTexture1D         | [**RWTexture1D**](sm5-object-rwtexture1d.md)                 |
| RasterizerOrderedTexture1DArray    | [**RWTexture1DArray**](sm5-object-rwtexture1darray.md)       |
| RasterizerOrderedTexture2D         | [**RWTexture2D**](sm5-object-rwtexture2d.md)                 |
| RasterizerOrderedTexture2DArray    | [**RWTexture2DArray**](sm5-object-rwtexture2darray.md)       |
| RasterizerOrderedTexture3D         | [**RWTexture3D**](sm5-object-rwtexture3d.md)                 |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модель шейдера 5,1](shader-model-5-1.md)
</dt> <dt>

[Функции HLSL Shader Model 5,1 для Direct3D 12](hlsl-shader-model-5-1-features-for-direct3d-12.md)
</dt> </dl>

 

 
