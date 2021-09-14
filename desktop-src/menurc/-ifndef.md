---
title: " ifndef"
description: Директива \ ifndef управляет условной компиляцией файла ресурсов путем проверки указанного имени.
ms.assetid: b83d7b0e-1a37-47a8-b495-0eab05ed3a9a
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 984a969123ea68fd68b14c1b98354b8bc5205aba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252451"
---
# <a name="ifndef"></a>\#ifndef

Директива **\# ifndef** управляет условной компиляцией файла ресурсов путем проверки указанного имени. Если имя не было определено или его определение было удалено с помощью директивы **\# undef** , то параметр **\# ifndef** указывает компилятору продолжить обработку операторов вплоть до следующей директивы **\# endif**, **\# else** или **\# elif** , а затем перейти к оператору после директивы **\# endif** . Если имя определено, то параметр **\# ifndef** направляет компилятор в следующую директиву **\# endif**, **\# else** или **\# elif** .

``` syntax
#ifndef name
```

<dl> <dt>

<span id="name"></span><span id="NAME"></span>*безымян*
</dt> <dd>

Имя, проверяемое директивой.

</dd> </dl>

## <a name="example"></a>Пример

Этот пример компилирует оператор [**Bitmap**](bitmap-resource.md) , только если не определен параметр optimize:

``` syntax
#ifndef Optimize
BITMAP 1 errbox.bmp
#endif
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Директивы препроцессора](preprocessor-directives.md)
</dt> </dl>

 

 




