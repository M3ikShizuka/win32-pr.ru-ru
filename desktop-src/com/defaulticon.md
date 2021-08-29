---
title: дефаултикон
description: Содержит сведения о значке по умолчанию для однообъектных презентаций.
ms.assetid: 45a3289b-d9c4-4857-bf48-1fd664ce4430
keywords:
- COM раздела реестра Дефаултикон
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 680994bdd4d4cd6ec6a3d192ca737af27f9190f6179571b3c8aaca5d86b55c5c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119501264"
---
# <a name="defaulticon"></a>дефаултикон

Содержит сведения о значке по умолчанию для однообъектных презентаций.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      DefaultIcon = path, resourceID
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ SZ** , указывающее полный путь к исполняемому файлу приложения объекта и индексу ресурса значка в исполняемом файле.

**Дефаултикон** определяет значок, используемый, если, например, элемент управления сведен к значку. Эта запись содержит полный путь к исполняемому файлу серверного приложения и индексу ресурса значка в исполняемом файле. Приложения могут использовать сведения, предоставляемые **дефаултикон** , для получения маркера значка с помощью [**екстрактикон**](/windows/win32/api/shellapi/nf-shellapi-extracticona).

 

 