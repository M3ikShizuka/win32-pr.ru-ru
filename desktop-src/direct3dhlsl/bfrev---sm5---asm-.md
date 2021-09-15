---
title: бфрев (SM5-ASM)
description: Обратный 32-разрядное число.
ms.assetid: 24F8209A-093E-4737-BF50-12F228024E9D
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 11bf0f07b6c66babf8e7f91108f86ba753420fc2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459217"
---
# <a name="bfrev-sm5---asm"></a>бфрев (SM5-ASM)

Обратный 32-разрядное число.



| бфрев dest \[ . Mask \] , src0 \[ . свиззле\] |
|---------------------------------------|



 



| Элемент                                                            | Описание:                                                  |
|-----------------------------------------------------------------|--------------------------------------------------------------|
| <span id="dest"></span><span id="DEST"></span>*dest*<br/> | \[в \] адресе для *src0* с обратным BITS.<br/> |
| <span id="src0"></span><span id="SRC0"></span>*src0*<br/> | \[в \] 32-разрядном числе для обращения.<br/>              |



 

## <a name="remarks"></a>Комментарии

Например, при наличии 0x12345678 результат будет 0x1e6a2c48.

Эта инструкция применяется к следующим этапам шейдера:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
| X      | X    | X      | X        | X     | X       |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта инструкция поддерживается в следующих моделях шейдеров:



| Модель шейдера                                              | Поддерживается |
|-----------------------------------------------------------|-----------|
| [Модель шейдера 5](d3d11-graphics-reference-sm5.md)        | Да       |
| [Модель шейдера 4,1](dx-graphics-hlsl-sm4.md)              | Нет        |
| [Модель шейдера 4](dx-graphics-hlsl-sm4.md)                | Нет        |
| [Модель шейдера 3 (DirectX HLSL)](dx-graphics-hlsl-sm3.md) | Нет        |
| [Модель шейдера 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) | Нет        |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md) | Нет        |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сборка Shader Model 5 (DirectX HLSL)](shader-model-5-assembly--directx-hlsl-.md)
</dt> </dl>

 

 





