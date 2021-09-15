---
title: Регистр счетчиков циклов (Справочник по HLSL VS)
description: Ознакомьтесь с регистром счетчиков циклов для шейдеров вершин. Единственный регистр в этом банке — регистрация текущего цикла (aL).
ms.assetid: b32fabf8-38d3-446c-bb80-c647d5aa028d
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 8fb728420dc48c6cb67d5973085845b0eab742a2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127581214"
---
# <a name="loop-counter-register-hlsl-vs-reference"></a>Регистр счетчиков циклов (Справочник по HLSL VS)

Единственный регистр в этом банке — регистрация текущего цикла (aL). Он автоматически увеличивается при каждом выполнении [цикла-VS](loop---vs.md).. блок [ендлуп-VS](endloop---vs.md) . Поэтому его можно использовать в блоке для относительной адресации, если это необходимо, и недопустимо использовать его за пределами цикла.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистры шейдеров вершин](dx9-graphics-reference-asm-vs-registers.md)
</dt> </dl>

 

 




