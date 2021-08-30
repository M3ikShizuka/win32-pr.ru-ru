---
description: 'Дополнительные сведения: JET_PCWSTR'
title: JET_PCWSTR
TOCTitle: JET_PCWSTR
ms:assetid: fef64bb9-c2e0-4cfb-8138-c98ae6f50952
ms:mtpsurl: https://msdn.microsoft.com/library/Gg294145(v=EXCHG.10)
ms:contentKeyID: 32765759
ms.date: 04/11/2016
ms.topic: reference
api_name: ''
topic_type:
- apiref
- kbArticle
api_type:
- COM
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: fa07aace787d8fdcc01b5fc4f5ac215f609f9f11
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122986107"
---
# <a name="jet_pcwstr"></a>JET_PCWSTR


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_pcwstr"></a>JET_PCWSTR

Тип данных **JET_PCWSTR** содержит константную строку в **Юникоде** , заканчивающуюся символом NULL \* .

**Windows vista: JET_PCWSTR** введены в Windows vista.

```cpp
    typedef __nullterminated const WCHAR * JET_PCWSTR;
```

### <a name="data-types"></a>Типы данных

JET_PCWSTR

Константа, заканчивающаяся символом NULL, строка Юникода (char \* ).

### <a name="requirements"></a>Требования


| Требование | Применение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows Server 2008.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 


