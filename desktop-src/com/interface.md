---
title: Interface (COM)
description: Необязательная запись, указывающая все идентификаторы интерфейса (идентификаторов IID), поддерживаемые связанным классом.
ms.assetid: 212a6500-14ce-4a9b-9e6a-38d83a5630c8
keywords:
- Раздел реестра интерфейса COM
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 990c06285d60067c9a26faffabffc70cbdd283d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126965217"
---
# <a name="interface-com"></a>Interface (COM)

Необязательная запись, указывающая все идентификаторы интерфейса (идентификаторов IID), поддерживаемые связанным классом.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      Interface
         {IID1} = name1
         {IID2} = name2
         ...
```

## <a name="remarks"></a>Комментарии

Если имя интерфейса отсутствует в этом списке, интерфейс не может поддерживаться экземпляром этого класса.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Ключ интерфейса](interface-key.md)
</dt> </dl>

 

 




