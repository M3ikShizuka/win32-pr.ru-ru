---
description: Свойство Волумесаваилабле извлекает количество томов в наборе из нескольких томов.
ms.assetid: d056b6d5-f4a4-480b-96a5-8e95dce23dfb
title: Волумесаваилабле, свойство
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ccdcf32ba8b7bea3958ef469bc0f90f9d41ecc14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272752"
---
# <a name="volumesavailable-property"></a>Волумесаваилабле, свойство

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`VolumesAvailable`Свойство получает количество томов в многотомном наборе.

``` syntax
[ iVolumes = ] MSWebDVD.VolumesAvailable
```

## <a name="return-value"></a>Возвращаемое значение

Возвращает количество томов в наборе в виде целого числа.

## <a name="remarks"></a>Комментарии

Это свойство доступно только для чтения и не имеет значения по умолчанию. Некоторые заголовки DVD могут быть выпущены в виде набора или ряда с несколькими дисками. Используйте этот метод, чтобы определить номер тома для текущего диска.

 

 



