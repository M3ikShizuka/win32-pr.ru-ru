---
description: 'Дополнительные сведения о: Есентрекорднотфаундексцептион Class'
title: Класс Есентрекорднотфаундексцептион
TOCTitle: EsentRecordNotFoundException class
ms:assetid: T:Microsoft.Isam.Esent.Interop.EsentRecordNotFoundException
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.esentrecordnotfoundexception(v=EXCHG.10)
ms:contentKeyID: 55102528
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.EsentRecordNotFoundException
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.EsentRecordNotFoundException
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: c013bda1ba0592b2137e4bc428ccf4bc195fc6ca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569582"
---
# <a name="esentrecordnotfoundexception-class"></a>Класс Есентрекорднотфаундексцептион

Базовый класс для JET_err. Исключения Рекорднотфаунд.

## <a name="inheritance-hierarchy"></a>Иерархия наследования

[System.Object](/dotnet/api/system.object)  
  [System.Exception](/dotnet/api/system.exception)  
    [Microsoft. ISAM. ESENT. Есентексцептион](./esentexception-class.md)  
      [Microsoft. ISAM. ESENT. Interop. Есентеррорексцептион](./esenterrorexception-class.md)  
        [Microsoft. ISAM. ESENT. Interop. Есентапиексцептион](./esentapiexception-class.md)  
          [Microsoft. ISAM. ESENT. Interop. Есентстатиксцептион](./esentstateexception-class.md)  
            Microsoft. ISAM. ESENT. Interop. Есентрекорднотфаундексцептион  

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
<SerializableAttribute> _
Public NotInheritable Class EsentRecordNotFoundException _
    Inherits EsentStateException
'Usage
Dim instance As EsentRecordNotFoundException
```

``` csharp
[SerializableAttribute]
public sealed class EsentRecordNotFoundException : EsentStateException
```

## <a name="thread-safety"></a>Потокобезопасность

Любые общедоступные статичные (общие в Visual Basic) члены этого типа являются потокобезопасными. Потокобезопасная работа с членами экземпляров типа не гарантируется.

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Ссылка

[Элементы Есентрекорднотфаундексцептион](./esentrecordnotfoundexception-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
