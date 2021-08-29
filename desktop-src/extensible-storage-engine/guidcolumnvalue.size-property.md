---
description: 'Дополнительные сведения о свойстве: Гуидколумнвалуе. size'
title: Гуидколумнвалуе. size, свойство
TOCTitle: 'Size property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.GuidColumnValue.Size
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.guidcolumnvalue.size(v=EXCHG.10)
ms:contentKeyID: 55107387
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.GuidColumnValue.Size
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.GuidColumnValue.get_Size
- Microsoft.Isam.Esent.Interop.GuidColumnValue.Size
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 3d9d5aa86f848485c4ce8ee61054e73894992192086a11e2388ed4c7b052295d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119039522"
---
# <a name="guidcolumnvaluesize-property"></a>Гуидколумнвалуе. size, свойство

Возвращает размер значения в столбце. Он возвращает 0 для столбцов переменного размера (т. е. двоичного и строкового).

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Protected Overrides ReadOnly Property Size As Integer
    Get
'Usage
Dim value As Integer

value = Me.Size
```

``` csharp
protected override int Size { get; }
```

#### <a name="property-value"></a>Значение свойства

Тип: [System. Int32](/dotnet/api/system.int32)  

## <a name="see-also"></a>См. также

#### <a name="reference"></a>Справочник

[Класс Гуидколумнвалуе](./guidcolumnvalue-class.md)

[Элементы Гуидколумнвалуе](./guidcolumnvalue-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
