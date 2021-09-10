---
title: дефаултикон
description: Содержит сведения о значке по умолчанию для однообъектных презентаций.
ms.assetid: 45a3289b-d9c4-4857-bf48-1fd664ce4430
keywords:
- COM раздела реестра Дефаултикон
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e0079fb02f4429c1939f54d643e0a6b08fbc90eb
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369581"
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

 

 