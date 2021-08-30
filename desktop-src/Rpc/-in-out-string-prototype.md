---
title: " в, out, строковый прототип"
description: В следующем прототипе функции для входных и выходных строк используется одиночный параметр "in", "out", "String \".
ms.assetid: 5a652b79-11ca-4780-aac1-60a22f96b4af
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 92fe0b2e39f6f3bda532b030cac1ec4c15a03b7bb5447401e0f1f43ebda466ab
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120024314"
---
# <a name="in-out-string-prototype"></a>\[в, out, строковый \] прототип

В приведенном ниже прототипе функции используется одиночный \[ [**строковый**](/windows/desktop/Midl/string) параметр [**in**](/windows/desktop/Midl/in) [**и**](/windows/desktop/Midl/out-idl) \] входных и выходных строк. Строка сначала содержит входные данные пациента, а затем переписывается с ответом Doctor, как показано ниже:

``` syntax
void Analyze([in, out, string, size_is(STRSIZE)] char  achInOut[]);
```

Этот пример похож на тот, который использовал строку с одной подсчетностью для ввода и вывода. Как и в этом примере, \[ [**атрибут \_ size**](/windows/desktop/Midl/size-is) \] определяет количество элементов, выделенных на сервере. Атрибут \[ [**String**](/windows/desktop/Midl/string) \] направляет заглушку вызывать **strlen** для определения числа переданных элементов.

Клиент выделяет всю память перед вызовом:

``` syntax
/* client */
char achInOut[STRSIZE];
...
gets_s(achInOut, STRSIZE);            // get patient input
Analyze(achInOut);
printf("%s\n", achInOut);  // display doctor response
```

Обратите внимание, что функция Analyze больше не должна вычислять длину возвращаемой строки, как в примере подсчета строки, где атрибут **\[ String \]** не использовался. Теперь суррогаты рассчитывают длину, как показано ниже:

``` syntax
/* server */
void Analyze(char *pchInOut)
{
   ...
   Respond(response, pchInOut); // don't need to call strlen
   return;                      // stubs handle size
}
```

 

 