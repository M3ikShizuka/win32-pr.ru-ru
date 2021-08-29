---
title: Представитель-PS
description: Запустить представителя... блок ендреп-PS.
ms.assetid: vs|directx_sdk|~\rep___ps.htm
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: ec879ad172b5cfc615a67797dd91c1461d844444326df6485b120179f6ecb74e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119853874"
---
# <a name="rep---ps"></a>Представитель-PS

Запустить представителя... блок [ендреп-PS](endrep---ps.md) .

## <a name="syntax"></a>Синтаксис



| Представитель\# |
|---------|



 

где i \# — это целочисленный регистр, указывающий число повторов в компоненте. x. См. раздел [Постоянный целочисленный регистр](dx9-graphics-reference-asm-ps-registers-constant-integer.md).

## <a name="remarks"></a>Remarks



| Версии шейдеров пикселей | 1\_1 | 1\_2 | 1 \_ 3 | 1\_4 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|-----------------------|------|------|------|------|------|------|-------|------|-------|
| склад                   |      |      |      |      |      | x    | x     | x    | x     |



 

-   i \# . x указывает число итераций. Допустимый диапазон: \[ 0, 255 \] . Обратите внимание, что эта инструкция не увеличивает или не уменьшает значение i \# . x.
-   i \# . ИЗВ не используются в блоке REPEAT.
-   Блоки Repeat могут быть вложенными. см. раздел [ограничения управления Flow](dx9-graphics-reference-asm-ps-instructions-flow-control.md).
-   Блоки Repeat могут быть либо полностью внутри \* блока if, либо полностью окружающи ее. Помещается в недопустимый.
-   Использование одного и того же i \# для различных или вложенных инструкций — Точная — каждый цикл выполняет итерацию в зависимости от указанного числа.

## <a name="example"></a>Пример


```
rep i2
    add r0, r0, c0
endrep  
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера пикселей](dx9-graphics-reference-asm-ps-instructions.md)
</dt> </dl>

 

 




