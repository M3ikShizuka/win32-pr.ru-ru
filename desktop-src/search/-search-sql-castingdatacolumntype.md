---
description: 'Дополнительные сведения: приведение типа данных столбца'
ms.assetid: 78a137a9-ef69-4ce3-8a96-73e722951300
title: Приведение типа данных столбца
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ad09572ca80ed433ebba63e84d4b7ca8bacdb6bd5cae45c356e358cbe978b04c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119094935"
---
# <a name="casting-the-data-type-of-a-column"></a>Приведение типа данных столбца

Иногда может потребоваться привести строковые данные, извлеченные из документов, в качестве другого типа данных, чтобы можно было выполнить соответствующее сравнение. Приведите идентификатор или литерал в качестве другого типа данных, используя следующий синтаксис:


```
CAST (<identifier> | <literal> AS <datatype>)
```



Пример:


```
CAST ('10000' AS DBTYPE_I4)
            
CAST (System.DateCreated AS DBTYPE_WSTR)
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сопоставление типов данных](-search-sql-datatypemappings.md)
</dt> </dl>

 

 



