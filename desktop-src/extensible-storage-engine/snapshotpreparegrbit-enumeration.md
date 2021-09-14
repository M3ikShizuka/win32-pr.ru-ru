---
description: Дополнительные сведения о перечислении Снапшотпрепарегрбит
title: Перечисление Снапшотпрепарегрбит
TOCTitle: SnapshotPrepareGrbit enumeration
ms:assetid: T:Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.snapshotpreparegrbit(v=EXCHG.10)
ms:contentKeyID: 39515688
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.CopySnapshot
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.IncrementalSnapshot
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.None
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.CopySnapshot
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.IncrementalSnapshot
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit.None
- Microsoft.Isam.Esent.Interop.SnapshotPrepareGrbit
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 32c11c609f78cc96862f9c2f15d93266f40ae941
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269619"
---
# <a name="snapshotpreparegrbit-enumeration"></a>Перечисление Снапшотпрепарегрбит

Параметры для [жетосснапшотпрепаре (JET_OSSNAPID, снапшотпрепарегрбит)](./api.jetossnapshotprepare-method.md).

Это перечисление имеет атрибут [FlagsAttribute](/dotnet/api/system.flagsattribute), который разрешает побитовое сочетание значений его элементов.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
<FlagsAttribute> _
Public Enumeration SnapshotPrepareGrbit
'Usage
Dim instance As SnapshotPrepareGrbit
```

``` csharp
[FlagsAttribute]
public enum SnapshotPrepareGrbit
```

## <a name="members"></a>Участники

<table>
<thead>
<tr class="header">
<th></th>
<th>Имя участника</th>
<th>Описание</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td></td>
<td>Нет</td>
<td>Параметры по умолчанию.</td>
</tr>
<tr class="even">
<td></td>
<td>IncrementalSnapshot</td>
<td>Будут предприняты только файлы журнала.</td>
</tr>
<tr class="odd">
<td></td>
<td>кописнапшот</td>
<td>Моментальный снимок копии (обычная или добавочная) без усечения журнала.</td>
</tr>
</tbody>
</table>


## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Справочник

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
