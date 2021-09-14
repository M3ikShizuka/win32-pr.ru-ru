---
title: Ресурс HTML
description: Определяет HTML-файл.
ms.assetid: d3cf8348-8c10-41d9-a061-cdce0e13abf4
keywords:
- Меню ресурсов HTML и другие ресурсы
topic_type:
- apiref
api_name:
- HTML
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9db6477aed5180ae18b99f53f4ebadf9d0ad0c91
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363512"
---
# <a name="html-resource"></a>Ресурс HTML

Определяет HTML-файл.

``` syntax
nameID HTML filename
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="nameID"></span><span id="nameid"></span><span id="NAMEID"></span>*nameID*
</dt> <dd>

Уникальное имя или 16-разрядное целочисленное значение без знака, идентифицирующее ресурс.

</dd> <dt>

<span id="filename"></span><span id="FILENAME"></span>*файлов*
</dt> <dd>

Имя HTML-файла. Он должен быть полным или относительным путем, если файл не находится в текущем рабочем каталоге. Путь должен представлять собой строку в кавычках.

</dd> </dl>

## <a name="examples"></a>Примеры

В следующем примере определяется ресурс HTML:

``` syntax
ID_RESPONSE_ERROR_PAGE  HTML "res\\responseerorpage.htm"
```

 

 




