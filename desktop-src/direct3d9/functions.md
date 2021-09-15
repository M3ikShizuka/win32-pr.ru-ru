---
description: Функция является стандартным блоком для шейдера, созданного на высоком уровне языка. Если вы предпочитаете писать шейдеры на языке C, а не на языке ассемблера, вам потребуется написать функции.
ms.assetid: vs|directx_sdk|~\functions.htm
title: Синтаксис функции Effect (Direct3D 9)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 21e239359877813e64acea8b5f404a6ade59c992
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127565986"
---
# <a name="effect-function-syntax-direct3d-9"></a>Синтаксис функции Effect (Direct3D 9)

Функция является стандартным блоком для шейдера, созданного на высоком уровне языка. Если вы предпочитаете писать шейдеры на языке C, а не на языке ассемблера, вам потребуется написать функции.

## <a name="syntax"></a>Синтаксис


```
type id ( [ parameters ] )  
    { body }
```



Функции не изменяют значения параметров в результате.

-   Type — любая допустимая [ссылка для типа HLSL](../direct3dhlsl/dx-graphics-hlsl-reference.md) .
-   ID — уникальное имя.
-   Parameters — параметры функции.
-   Body — текст функции.

Функции основаны на высоком уровне языка. См. [Справочник по HLSL](../direct3dhlsl/dx-graphics-hlsl-reference.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Формат эффектов](dx9-graphics-reference-effects-file-format.md)
</dt> </dl>

 

 
