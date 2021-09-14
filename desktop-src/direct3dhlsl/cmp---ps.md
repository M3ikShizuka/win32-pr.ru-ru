---
title: CMP-PS
description: Выберите src1, если src0 0. В противном случае выберите src2. Сравнение выполняется по каналу.
ms.assetid: 8fabd548-3f5e-4b78-bf1e-16e4f1548ccd
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: da3da1062d02e995876a1f67e5c4e19518774760
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264368"
---
# <a name="cmp---ps"></a>CMP-PS

Выберите src1, если src0 >= 0. В противном случае выберите src2. Сравнение выполняется по каналу.

## <a name="syntax"></a>Синтаксис



| CMP DST, src0, src1, src2 |
|---------------------------|



 

где

-   DST — это регистр назначения.
-   src0 является исходным регистром.
-   src1 является исходным регистром.
-   src2 является исходным регистром.

## <a name="remarks"></a>Remarks



| Версии шейдеров пикселей | 1\_1 | 1\_2 | 1 \_ 3 | 1\_4 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|-----------------------|------|------|------|------|------|------|-------|------|-------|
| файле                   |      | x    | x    | x    | x    | x    | x     | x    | x     |



 

Существует несколько дополнительных ограничений для версий 1 \_ 2 и 1 \_ 3:

-   Каждый шейдер может использовать не более трех инструкций CMP.
-   Регистр назначения не может совпадать с исходным регистром.

В этом примере выполняется сравнение четырех каналов.


```
ps_1_4
def c0, -0.6, 0.6, 0, 0.6
def c1  0,0,0,0
def c2  1,1,1,1

mov r1, c1
mov r2, c2

cmp r0, c0, r1, r2   // r0 is assigned 1,0,0,0 based on the following:

// r0.x = c2.x because c0.x < 0
// r0.y = c1.y because c0.y >= 0
// r0.z = c1.z because c0.z >= 0
// r0.w = c1.w because c0.w >= 0
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера пикселей](dx9-graphics-reference-asm-ps-instructions.md)
</dt> </dl>

 

 




