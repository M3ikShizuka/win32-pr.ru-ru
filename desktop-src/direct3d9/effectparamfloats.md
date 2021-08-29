---
description: Определяет действующие числа с плавающей запятой. Этот шаблон заменяет шаблон Еффектфлоатс.
ms.assetid: 7b41d0dc-209f-4ade-a7ed-aa54f421e520
title: еффектпарамфлоатс
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3f34f60c16f583021d0e7f01482941fa31d12861d4a59c07c26c7aa89a96e3d9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119122393"
---
# <a name="effectparamfloats"></a>еффектпарамфлоатс

Определяет действующие числа с плавающей запятой. Этот шаблон заменяет шаблон [**еффектфлоатс**](effectfloats.md) .

``` syntax
template EffectParamFloats
{
    < 3014B9A0-62F5-478c-9B86-E4AC9F4E418B >
    STRING ParamName;
    DWORD nFloats;
    array float Floats[nFloats];
} 
```

Где:

-   ParamName — имя массива чисел с плавающей запятой.
-   Нфлоатс — число значений с плавающей запятой в массиве.
-   \[ \] Массивы с плавающей запятой нфлоатс.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Шаблоны](dx9-graphics-reference-x-file-format-templates.md)
</dt> </dl>

 

 



