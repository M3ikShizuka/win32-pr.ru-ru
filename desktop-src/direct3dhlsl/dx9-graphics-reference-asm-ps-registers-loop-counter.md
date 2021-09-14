---
title: Регистр счетчиков циклов (Справочник по HLSL PS)
description: Ознакомьтесь с регистром счетчиков циклов для шейдеров пикселей. Единственный регистр в этом банке — регистрация текущего цикла (aL).
ms.assetid: 36999873-a251-4939-aac0-faa7f910bc33
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: b2a2f7f42c83308fa72ceae2875c35c600dfd7db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264016"
---
# <a name="loop-counter-register-hlsl-ps-reference"></a>Регистр счетчиков циклов (Справочник по HLSL PS)

Единственный регистр в этом банке — регистрация текущего цикла (aL). Он автоматически увеличивается при каждом выполнении блока [Loop-PS](loop---ps.md) / [ендлуп-PS](endloop---ps.md) . Поэтому его можно использовать в блоке для относительной адресации, если это необходимо, и недопустимо использовать его за пределами цикла.



| Версии шейдеров пикселей | 1\_1 | 1\_2 | 1 \_ 3 | 1\_4 | 2 \_ 0 | 2 \_ SW | 2 \_ x | 3 \_ 0 | 3 \_ SW |
|-----------------------|------|------|------|------|------|-------|------|------|-------|
| Регистр счетчика цикла |      |      |      |      |      |       |      | x    | x     |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистры](dx9-graphics-reference-asm-ps-registers.md)
</dt> </dl>

 

 




