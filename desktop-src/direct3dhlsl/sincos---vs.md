---
title: синкос — VS
description: Вычисляет синус и косинус в радианах. | синкос — VS
ms.assetid: 733a3980-ceaf-43dc-a862-923c369e4a65
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: ca70a319852346c6e75ba544489d033a861d4c3b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127263904"
---
# <a name="sincos---vs"></a>синкос — VS

Вычисляет синус и косинус в радианах.

## <a name="syntax"></a>Синтаксис

### <a name="vs_2_0-and-vs_2_x"></a>VS \_ 2 \_ 0 и VS \_ 2 \_ x



| синкос DST. x|&|XY}, src0. x|&|гармошкой|w}, src1, src2 |
|------------------------------------------------------|



 

Где:

-   DST — это регистр назначения, который должен быть [временным регистром](dx9-graphics-reference-asm-vs-registers-temporary.md) (r \# ). Регистр назначения должен иметь ровно одну из трех масок:. x \| . y \| . XY.
-   src0 — это исходный регистр, который предоставляет угол ввода, который должен быть в пределах \[ -Pi, + PI \] . {x \| y \| z \| w} — это требуемая репликация свиззле.
-   src1 и src2 являются исходными регистрами и должны быть двумя разными [константами регистра с плавающей запятой](dx9-graphics-reference-asm-vs-registers-constant-float.md) (c \# ). Значения src1 и src2 должны относиться к макросам [**D3DSINCOSCONST1**](/windows/desktop/direct3d9/d3dsincosconst1) и [**D3DSINCOSCONST2**](/windows/desktop/direct3d9/d3dsincosconst2) соответственно.

### <a name="vs_3_0"></a>VS \_ 3 \_ 0



| синкос DST. x|&|XY}, src0. x|&|гармошкой|Белая |
|------------------------------------------|



 

Где:

-   DST — это регистр назначения, который должен быть [временным регистром](dx9-graphics-reference-asm-vs-registers-temporary.md) (r \# ). Регистр назначения должен иметь ровно одну из трех масок:. x \| . y \| . XY.
-   src0 — это исходный регистр, который предоставляет угол ввода, который должен быть в пределах \[ -Pi, + PI \] . {x \| y \| z \| w} — это требуемая репликация свиззле.

## <a name="remarks"></a>Remarks



| Версии шейдеров вершин | 1\_1 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|------------------------|------|------|------|-------|------|-------|
| синкос                 |      | x    | x    | x     | x    | x     |



 

### <a name="vs_2_0-and-vs_2_x-remarks"></a>\_Примечания vs 2 \_ 0 и VS \_ 2 \_ x

Для VS \_ 2 \_ 0 и VS \_ 2 \_ x синкос можно использовать с затенения, но с одним ограничением на свиззле [регистра предиката](dx9-graphics-reference-asm-vs-registers-predicate.md) (P0): допускается только репликация свиззле (. x \| . y \| . z \| . w).

Для VS \_ 2 \_ 0 и VS \_ 2 \_ x инструкция работает следующим образом: (V = скалярное значение из src0 с реплицируемой свиззле):

-   Если маска записи —. x:
    ```
    dest.x = cos( V )
    dest.y is undefined when the instruction completes
    dest.z is undefined when the instruction completes
    dest.w is not touched by the instruction
    ```

    

-   Если маска записи —. y:
    ```
    dest.x is undefined when the instruction completes
    dest.y = sin( V )
    dest.z is undefined when the instruction completes
    dest.w is not touched by the instruction
    ```

    

-   Если маска записи имеет значение. XY:
    ```
    dest.x = cos( V )
    dest.y = sin( V )
    dest.z is undefined when the instruction completes
    dest.w is not touched by the instruction
    ```

    

### <a name="vs_3_0-remarks"></a>\_Примечание VS 3 \_ 0

Для VS \_ 3 \_ 0 синкос можно использовать с затенения без каких бы то ни было ограничений. См. раздел [Регистрация предиката](dx9-graphics-reference-asm-vs-registers-predicate.md).

Для VS \_ 3 \_ 0 Инструкция работает следующим образом: (V = скалярное значение из src0 с репликацией свиззле).

-   Если маска записи —. x:
    ```
    dest.x = cos( V )
    dest.y is not touched by the instruction
    dest.z is not touched by the instruction
    dest.w is not touched by the instruction
    ```

    

-   Если маска записи —. y:
    ```
    dest.x is not touched by the instruction
    dest.y = sin( V )
    dest.z is not touched by the instruction
    dest.w is not touched by the instruction
    ```

    

-   Если маска записи имеет значение. XY:
    ```
    dest.x = cos( V )
    dest.y = sin( V )
    dest.z is not touched by the instruction
    dest.w is not touched by the instruction
    ```

    

Приложение может сопоставлять произвольный угол (в радианах) с Range \[ -Pi, + PI, \] используя следующий псевдокод шейдера:


```
def c0, pi, 0.5, 2*pi, 1/(2*pi)
mad r0.x, input_angle, c0.w, c0.y
frc r0.x, r0.x
mad r0.x, r0.x, c0.z, -c0.x
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера вершин](dx9-graphics-reference-asm-vs-instructions.md)
</dt> </dl>

 

 
