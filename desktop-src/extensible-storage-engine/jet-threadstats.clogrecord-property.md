---
description: 'Дополнительные сведения о свойстве: JET_THREADSTATS. Клогрекорд'
title: Свойство JET_THREADSTATS. Клогрекорд (Microsoft. ISAM. ESENT. Interop. Vista)
TOCTitle: 'cLogRecord property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cLogRecord
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.vista.jet_threadstats.clogrecord(v=EXCHG.10)
ms:contentKeyID: 39511382
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cLogRecord
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cLogRecord
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.get_cLogRecord
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.set_cLogRecord
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 17947c0ea74f00ae51101d3e10b2eb54c78abe7a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126962793"
---
# <a name="jet_threadstatsclogrecord-property"></a>Свойство JET_THREADSTATS. Клогрекорд

Возвращает общее число записей журнала транзакций, созданных ядром СУБД в текущем потоке.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Property cLogRecord As Integer
    Get
    Friend Set
'Usage
Dim instance As JET_THREADSTATS
Dim value As Integer

value = instance.cLogRecord
```

``` csharp
public int cLogRecord { get; internal set; }
```

#### <a name="property-value"></a>Значение свойства

Тип: [System. Int32](/dotnet/api/system.int32)  

## <a name="see-also"></a>См. также:

#### <a name="reference"></a>Справочник

[Структура JET_THREADSTATS](./jet-threadstats-structure2.md)

[Элементы JET_THREADSTATS](./jet-threadstats-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)
