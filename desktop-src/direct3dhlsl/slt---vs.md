---
title: SLT — VS
description: Подсчитывает знак, если первый источник меньше второго источника.
ms.assetid: 7573bcee-8f31-49ea-b515-5be59a7a508d
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: f6476ec24f82295d56b04682dfa4320547672b43
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459188"
---
# <a name="slt---vs"></a>SLT — VS

Подсчитывает знак, если первый источник меньше второго источника.

## <a name="syntax"></a>Синтаксис



| SLT DST, src0, src1 |
|---------------------|



 

где

-   DST — это регистр назначения.
-   src0 является исходным регистром.
-   src1 является исходным регистром.

## <a name="remarks"></a>Комментарии



| Версии шейдеров вершин | 1\_1 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|------------------------|------|------|------|-------|------|-------|
| SLT                    | x    | x    | x    | x     | x    | x     |



 

В следующем фрагменте кода показаны выполняемые операции.


```
dest.x = (src0.x < src1.x) ? 1.0f : 0.0f;
dest.y = (src0.y < src1.y) ? 1.0f : 0.0f;
dest.z = (src0.z < src1.z) ? 1.0f : 0.0f;
dest.w = (src0.w < src1.w) ? 1.0f : 0.0f;
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Инструкции шейдера вершин](dx9-graphics-reference-asm-vs-instructions.md)
</dt> </dl>

 

 




