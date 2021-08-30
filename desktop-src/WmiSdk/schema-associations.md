---
description: 'В запросах сопоставления схем используются те же инструкции, что и в запросах ассоциаций данных: СОЕДИНИТЕЛи и ссылки.'
ms.assetid: b5fc2d86-702a-42cd-82e6-f15c905ba6aa
ms.tgt_platform: multiple
title: Сопоставления схем
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 461dc7c64267376baf1515ed7784da59bc789f6f1cc1171587823adb27799830
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119995694"
---
# <a name="schema-associations"></a>Сопоставления схем

В запросах сопоставления схем используются те же инструкции, что и в запросах ассоциаций данных: СОЕДИНИТЕЛи и ссылки. Однако при использовании запросов ассоциаций данных возвращаются экземпляры классов, а с запросами связей схем — имена классов, которые могут участвовать в отношениях взаимосвязей. Например, можно использовать запрос схемы для поиска всех классов взаимосвязей, определенных в схеме, ссылающейся на исходный класс.

Синтаксис для СОЕДИНИТЕЛей и ссылок на инструкции одинаков для запросов связи схемы, так как он предназначен для запросов ассоциаций данных со следующими исключениями:

-   Исходный объект является классом, а не экземпляром.
-   Существует дополнительное ключевое слово **SchemaOnly**, которое определяет запрос как применяемый к схеме, а не к данным.
-   Недопустимое ключевое слово **классдефсонли** .

В следующем примере показан полный синтаксис СОЕДИНИТЕЛей оператора для запроса схемы. Подробный синтаксис см. в разделе [соединители оператора](associators-of-statement.md).


```sql
ASSOCIATORS OF {SourceClass} WHERE 
    AssocClass = AssocClassName
    RequiredAssocQualifier = QualifierName
    RequiredQualifier = QualifierName
    ResultClass = ClassName
    ResultRole = PropertyName
    Role = PropertyName
    SchemaOnly
```



В следующем примере показан запрос, возвращающий классы **протокола** и **драйвера** , два класса, которые ссылаются на исходный класс.


```sql
ASSOCIATORS OF {Adapter} WHERE SchemaOnly
```



Следующий запрос возвращает только класс **Driver** из-за ограничения, накладываемого ключевым словом **ассоккласс** .


```sql
ASSOCIATORS OF {Adapter} WHERE AssocClass = AdapterDriver SchemaOnly
```



Полный синтаксис ссылок на инструкцию для запроса схемы выглядит следующим образом. Подробный синтаксис см. в разделе [ссылки на инструкцию](references-of-statement.md).


```sql
REFERENCES OF {SourceClass} WHERE
    ResultClass = ClassName
    Role = PropertyName
    RequiredQualifier = QualifierName
    SchemaOnly
```



> [!Note]  
> Запросы связей схем могут возвращать дубликаты объектов.

 

Например, следующий запрос будет возвращать класс [**CIM \_ ComputerSystem**](/windows/desktop/CIMWin32Prov/cim-computersystem) несколько раз при перечислении классов в **корневом пространстве имен \\ CIMV2** .


```sql
ASSOCIATORS OF {Win32_ComputerSystem} WHERE SchemaOnly
```



 

 
