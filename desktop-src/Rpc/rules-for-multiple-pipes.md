---
title: Правила для нескольких каналов
description: Правила для нескольких каналов в одном вызове в удаленном вызове процедур (RPC).
ms.assetid: 1d0b2aed-27cc-4e74-9307-ada86bda4596
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0d804c132d7fc859906f065e4c9dc39dd3159519
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461522"
---
# <a name="rules-for-multiple-pipes"></a>Правила для нескольких каналов

В \[ [](/windows/desktop/Midl/in) \] \[ [](/windows/desktop/Midl/out-idl) \] \[  \] любом сочетании в одном вызове можно сочетать параметры вертикального канала, out и in, но необходимо обработать каналы в определенном порядке, как показано в следующем примере псевдокода:

> [!Note]  
> эта функция больше не поддерживается в Windows Vista и более поздних платформах.

 

-   Получите данные из каждого входного канала, начиная с первого (крайнего левого) \[ **в** \] параметре, и продолжая по порядку выполнять сток каждого канала перед началом обработки следующего.
-   После полной обработки каждого входного канала отправьте данные для выходных каналов, снова начиная с первого \[ **выходного** \] параметра и продолжая по порядку, заполняя каждый канал перед началом обработки следующего.

``` syntax
//in .IDL file:
void InOutUCharPipe( [in,out] UCHAR_PIPE *uchar_pipe_1, 
                     [out] UCHAR_PIPE * uchar_pipe_2, 
                     [in] UCHAR_PIPE uchar_pipe_3);
 
//remote procedure:
void InOutUCharPipe( UCHAR_PIPE *param1,
                     UCHAR_PIPE *param2,
                     UCHAR_PIPE  param3)
{
    while(!END_OF_PIPE1)
    {
        param1->pull (. . .);
        . . .
    };

    while(!END_OF_PIPE3)
    {
        param3.pull (. . .);
        . . .
    };

    while(!END_OF_PIPE1)
    {
        param1->push (. . .);
        . . .
    };

    while(!END_OF_PIPE2)
    {
        param2->push(. . .);
        . . .
    };
} //end InOutUCharPipe
```

 

 