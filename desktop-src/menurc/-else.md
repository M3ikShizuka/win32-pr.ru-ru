---
title: " else"
description: Директива \ else помечает необязательное предложение блока условной компиляции, определенного директивой \ ifdef, \ ifndef или \ if. Директива \ else должна быть последней директивой перед директивой \ endif.
ms.assetid: 982466d9-ae77-4e1c-89f3-511335165da7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: aade46f8d2af211d4ed09e596ec3a42fa57d141d3d533bdbe34be09d9e9988c3
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120060204"
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

 

 




