---
title: Оболочка (COM)
description: обеспечивает Windowsную печать оболочки 3,1 и сведения о его открытии.
ms.assetid: 15e329f2-ed64-4940-aa00-63edbd283b07
keywords:
- COM-сценарий раздела реестра оболочки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 93ebbc83642896aa22f33b315e26097760f7311ec93d938cb0440a10e0aae049
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119129906"
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

 

 




