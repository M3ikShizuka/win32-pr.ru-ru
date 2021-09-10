---
title: Control
description: определяет объект как элемент управления ActiveX.
ms.assetid: 2487e642-1d21-4811-87dd-b280be98a44b
keywords:
- Управление ключом реестра COM
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3722d85b38399d7e95f226749bda45ccc82d1369
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369577"
---
# <a name="control"></a>Control

определяет объект как элемент управления ActiveX.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      Control
```

## <a name="remarks"></a>Remarks

Эта необязательная запись используется контейнерами для заполнения диалоговых окон. контейнер использует этот подраздел, чтобы определить, следует ли включать объект в диалоговое окно, в котором отображаются элементы управления ActiveX. Элемент управления может опускать эту запись, если она предназначена для работы только с конкретным контейнером и поэтому не предназначена для вставки в другие контейнеры.

 

 




