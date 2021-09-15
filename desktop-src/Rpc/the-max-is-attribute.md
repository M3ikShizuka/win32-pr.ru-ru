---
title: Атрибут max_is
description: Можно указать допустимые границы для индексных номеров массива, используя атрибут \ Max = \_ \.
ms.assetid: b629e3cf-544d-47ee-8f8f-b049f693897c
keywords:
- max_is
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8901f952a55de6b81143b0e615c878d8599fb354
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470026"
---
# <a name="the-max_is-attribute"></a>\[Атрибут Max \_ — \]

Можно указать допустимые границы для номеров индексов массива с помощью \[ атрибута [**Max \_**](/windows/desktop/Midl/max-is) \] .

``` syntax
/* IDL file */
[ 
  uuid(ba209999-0c6c-11d2-97cf-00c04f8eea45),
  version(5.0)
]
interface arraytest
{
  void fArray5([in] short sMax,
               [in, out, max_is(sMax)]  char achArray[]);
}
```

 

 