---
title: " else"
description: Директива \ else помечает необязательное предложение блока условной компиляции, определенного директивой \ ifdef, \ ifndef или \ if. Директива \ else должна быть последней директивой перед директивой \ endif.
ms.assetid: 982466d9-ae77-4e1c-89f3-511335165da7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 086acd9e6323f7be11a65951a33b2b11b680ad46
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252460"
---
# <a name="else"></a>\#Кроме

Директива **\# else** помечает необязательное предложение блока условной компиляции, определенного директивой **\# ifdef**, **\# ifndef** или **\# If** . Директива **\# else** должна быть последней директивой перед директивой **\# endif** .

``` syntax
#else
```

Эта директива не имеет параметров.

## <a name="example"></a>Пример

Этот пример компилирует второй оператор [**Bitmap**](bitmap-resource.md) , только если не ОПРЕДЕЛЕН параметр debug:

``` syntax
#ifdef DEBUG
    BITMAP 1 errbox.bmp
#else
    BITMAP 1 userbox.bmp
#endif
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Директивы препроцессора](preprocessor-directives.md)
</dt> </dl>

 

 




