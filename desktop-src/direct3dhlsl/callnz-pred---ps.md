---
title: каллнз, пред-PS
description: Вызов с предикатом, если он не равен нулю. Выполняет условный вызов инструкции, помеченной индексом метки. Затенения использует логическое значение, чтобы определить, не нужно ли выполнять инструкцию.
ms.assetid: 9c839fc7-8b4d-4ca1-b30f-5c3f8fb45eae
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: a04bd4b1bfa16d965a90b66e3956674ecb112590
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574006"
---
# <a name="callnz-pred---ps"></a>каллнз, пред-PS

Вызов с предикатом, если он не равен нулю. Выполняет условный вызов инструкции, помеченной индексом метки. Затенения использует логическое значение, чтобы определить, не нужно ли выполнять инструкцию.

## <a name="syntax"></a>Синтаксис



| каллнз l \# , \[ ! \] P0. x|&|гармошкой|Белая |
|----------------------------------|



 

Где:

-   где l \# — [Метка-PS](label---ps.md) , помечающая начало подпрограммы для вызова.
-   \[!\] является необязательным модификатором отрицания.
-   P0 — это регистр предикатов. См. раздел [Регистрация предиката](dx9-graphics-reference-asm-ps-registers-predicate.md).
-   {x \| y \| z \| w} — это обязательная репликация свиззле в P0.

## <a name="remarks"></a>Комментарии



| Версии шейдеров пикселей | 1\_1 | 1\_2 | 1 \_ 3 | 1\_4 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|-----------------------|------|------|------|------|------|------|-------|------|-------|
| каллнз, пред.           |      |      |      |      |      | x    | x     | x    | x     |



 

Эта инструкция выполняет следующие действия:


```
if (specified register component is not zero)
{
    Push address of the next instruction to the return address stack
    Continue execution from the instruction marked by the label
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера пикселей](dx9-graphics-reference-asm-ps-instructions.md)
</dt> </dl>

 

 




