---
title: Оболочка (COM)
description: обеспечивает Windowsную печать оболочки 3,1 и сведения о его открытии.
ms.assetid: 15e329f2-ed64-4940-aa00-63edbd283b07
keywords:
- COM-сценарий раздела реестра оболочки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1acf4a62d72892d1cd25a5f2276e71d52ab7f700
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127457947"
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

## <a name="remarks"></a>Комментарии

Эти записи должны предоставить путь и имя файла приложения.

 

 




