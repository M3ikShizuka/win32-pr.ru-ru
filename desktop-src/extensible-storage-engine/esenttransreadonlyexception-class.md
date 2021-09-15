---
description: 'Дополнительные сведения о: Есенттрансреадонлексцептион Class'
title: Класс Есенттрансреадонлексцептион
TOCTitle: EsentTransReadOnlyException class
ms:assetid: T:Microsoft.Isam.Esent.Interop.EsentTransReadOnlyException
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.esenttransreadonlyexception(v=EXCHG.10)
ms:contentKeyID: 55107336
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.EsentTransReadOnlyException
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.EsentTransReadOnlyException
topic_type:
- apiref
- kbSyntax
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: eeb3576b2c33356c942e427d92bc40697c09921a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567026"
---
# <a name="esenttransreadonlyexception-class"></a>Класс Есенттрансреадонлексцептион

Базовый класс для JET_err. Исключения с модификатором ReadOnly.

## <a name="inheritance-hierarchy"></a>Иерархия наследования

[System.Object](/dotnet/api/system.object)  
  [System.Exception](/dotnet/api/system.exception)  
    [Microsoft. ISAM. ESENT. Есентексцептион](./esentexception-class.md)  
      [Microsoft. ISAM. ESENT. Interop. Есентеррорексцептион](./esenterrorexception-class.md)  
        [Microsoft. ISAM. ESENT. Interop. Есентапиексцептион](./esentapiexception-class.md)  
          [Microsoft. ISAM. ESENT. Interop. Есентусажеексцептион](./esentusageexception-class.md)  
            Microsoft. ISAM. ESENT. Interop. Есенттрансреадонлексцептион  

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
<SerializableAttribute> _
Public NotInheritable Class EsentTransReadOnlyException _
    Inherits EsentUsageException
'Usage
Dim instance As EsentTransReadOnlyException
```

``` csharp
[SerializableAttribute]
public sealed class EsentTransReadOnlyException : EsentUsageException
```

## <a name="thread-safety"></a>Потокобезопасность

Любые общедоступные статичные (общие в Visual Basic) члены этого типа являются потокобезопасными. Потокобезопасная работа с членами экземпляров типа не гарантируется.

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Ссылка

[Элементы Есенттрансреадонлексцептион](./esenttransreadonlyexception-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
