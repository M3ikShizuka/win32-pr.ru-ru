---
description: 'Дополнительные сведения: JET_PWSTR'
title: JET_PWSTR
TOCTitle: JET_PWSTR
ms:assetid: 6575f0f0-d022-4e70-9f17-c1d884d9e226
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269271(v=EXCHG.10)
ms:contentKeyID: 32765573
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
ms.openlocfilehash: adfa30d90087113f14b684440c21d6246fdc1f64
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122987847"
---
# <a name="jet_pwstr"></a>JET_PWSTR


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_pwstr"></a>JET_PWSTR

Тип данных **JET_PWSTR** содержит строку в **Юникоде** , заканчивающуюся символом NULL \* .

**Windows vista: JET_PWSTR** введены в Windows vista.

```cpp
    typedef __nullterminated WCHAR * JET_PWSTR;
```

### <a name="data-types"></a>Типы данных

JET_PWSTR

Заканчивающийся нулем, строка в Юникоде (char \* ).

### <a name="requirements"></a>Требования


| Требование | Применение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows Server 2008.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 


