---
description: 'Дополнительные сведения о: JET_CONDITIONALCOLUMN классе'
title: Класс JET_CONDITIONALCOLUMN
TOCTitle: JET_CONDITIONALCOLUMN class
ms:assetid: T:Microsoft.Isam.Esent.Interop.JET_CONDITIONALCOLUMN
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.jet_conditionalcolumn(v=EXCHG.10)
ms:contentKeyID: 55107506
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.JET_CONDITIONALCOLUMN
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.JET_CONDITIONALCOLUMN
topic_type:
- apiref
- kbSyntax
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 79a93eb5f5ffe0d13f78f5d387b37c4d17bd969a697dfb11998f5d7dcc821f1b
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120017624"
---
# <a name="jet_conditionalcolumn-class"></a>Класс JET_CONDITIONALCOLUMN

Определяет, как выполняется условное индексирование для данного индекса. Условный индекс содержит элемент индекса только для тех строк, которые соответствуют заданному условию. Однако условный столбец не является частью ключа индекса, он только управляет присутствием элемента индекса.

## <a name="inheritance-hierarchy"></a>Иерархия наследования

[System.Object](/dotnet/api/system.object)  
  Microsoft.Isam.Esent.Interop.JET_CONDITIONALCOLUMN  

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
<SerializableAttribute> _
Public NotInheritable Class JET_CONDITIONALCOLUMN _
    Implements IContentEquatable(Of JET_CONDITIONALCOLUMN), IDeepCloneable(Of JET_CONDITIONALCOLUMN)
'Usage
Dim instance As JET_CONDITIONALCOLUMN
```

``` csharp
[SerializableAttribute]
public sealed class JET_CONDITIONALCOLUMN : IContentEquatable<JET_CONDITIONALCOLUMN>, 
    IDeepCloneable<JET_CONDITIONALCOLUMN>
```

## <a name="thread-safety"></a>Потокобезопасность

Любые общедоступные статичные (общие в Visual Basic) члены этого типа являются потокобезопасными. Потокобезопасная работа с членами экземпляров типа не гарантируется.

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Справочник

[Элементы JET_CONDITIONALCOLUMN](./jet-conditionalcolumn-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
