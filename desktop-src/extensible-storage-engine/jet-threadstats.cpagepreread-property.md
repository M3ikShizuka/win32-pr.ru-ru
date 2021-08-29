---
description: 'Дополнительные сведения о свойстве: JET_THREADSTATS. Кпажепререад'
title: Свойство JET_THREADSTATS. Кпажепререад (Microsoft. ISAM. ESENT. Interop. Vista)
TOCTitle: 'cPagePreread property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cPagePreread
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.vista.jet_threadstats.cpagepreread(v=EXCHG.10)
ms:contentKeyID: 39510638
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cPagePreread
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.get_cPagePreread
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.cPagePreread
- Microsoft.Isam.Esent.Interop.Vista.JET_THREADSTATS.set_cPagePreread
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: bdbdcce28ecbe0cccb4739334cd9f5c2a2610875f2a6687aa71e9358f63bd065
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119832644"
---
# <a name="jet_threadstatscpagepreread-property"></a>Свойство JET_THREADSTATS. Кпажепререад

Возвращает общее число страниц базы данных, выбранных с диска ядром СУБД в текущем потоке.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Property cPagePreread As Integer
    Get
    Friend Set
'Usage
Dim instance As JET_THREADSTATS
Dim value As Integer

value = instance.cPagePreread
```

``` csharp
public int cPagePreread { get; internal set; }
```

#### <a name="property-value"></a>Значение свойства

Тип: [System. Int32](/dotnet/api/system.int32)  

## <a name="see-also"></a>См. также

#### <a name="reference"></a>Справочник

[Структура JET_THREADSTATS](./jet-threadstats-structure2.md)

[Элементы JET_THREADSTATS](./jet-threadstats-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)
