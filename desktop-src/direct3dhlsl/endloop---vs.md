---
title: ендлуп — VS
description: Конец цикла... блок ендлуп.
ms.assetid: fd7df120-a927-4a66-b152-6ce5247446e4
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 8a9aec4d1b2c5237a87fae2c0beab4e8d995db97
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066177"
---
# <a name="endloop---vs"></a>ендлуп — VS

Конец [цикла](loop---vs.md)... блок ендлуп.

## <a name="syntax"></a>Синтаксис



| ендлуп |
|---------|



 

## <a name="remarks"></a>Remarks



| Версии шейдеров вершин | 1\_1 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|------------------------|------|------|------|-------|------|-------|
| ендлуп                |      | x    | x    | x     | x    | x     |



 

Эта инструкция работает, как показано здесь.


```
LoopCounter += LoopStep;
LoopInterationCount = LoopIterationCount - 1;
if (LoopIterationCount > 0)
    Continue execution at the StartLoopOffset
```



ендлуп должен следовать последней инструкции блока [цикла VS](loop---vs.md) .

## <a name="example"></a>Пример


```
loop aL, i3
    add r1, r0, c2[ aL ]
endloop
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера вершин](dx9-graphics-reference-asm-vs-instructions.md)
</dt> </dl>

 

 




