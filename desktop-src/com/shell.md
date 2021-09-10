---
title: Оболочка (COM)
description: обеспечивает Windowsную печать оболочки 3,1 и сведения о его открытии.
ms.assetid: 15e329f2-ed64-4940-aa00-63edbd283b07
keywords:
- COM-сценарий раздела реестра оболочки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1acf4a62d72892d1cd25a5f2276e71d52ab7f700
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369478"
---
# <a name="shell-com"></a>Оболочка (COM)

обеспечивает Windowsную печать оболочки 3,1 и сведения о его **открытии** .

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes
   {ProgID}
      Shell
         Open
            command = path %1
         Print
            command = path %1
```

## <a name="remarks"></a>Remarks

Эти записи должны предоставить путь и имя файла приложения.

 

 




