---
description: Свойство Volume задает или получает громкость динамика для выходных данных аудиопотока.
ms.assetid: b6e22d07-525b-4af2-898c-ce3ed16ea9c1
title: Свойство Volume
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0c9c85bc2d20a613e61d454f75b9663284188c16
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272755"
---
# <a name="volume-property"></a>Свойство Volume

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`Volume`Свойство задает или получает громкость динамика для выходных данных аудиопотока.

``` syntax
[ iVolume = ] MSWebDVD.Volume
```

## <a name="return-value"></a>Возвращаемое значение

Возвращает уровень громкости в виде затухания в децибел в виде целого числа.

## <a name="remarks"></a>Комментарии

Это свойство доступно для чтения и записи со значением по умолчанию 0. Полный том равен 0, а 10 000 — тишина; шкала является логарифмической. Умножьте требуемый уровень шкала на 100 (например, 10 000 = 100 dB).

 

 



