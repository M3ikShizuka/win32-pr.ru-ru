---
description: 'Дополнительные сведения о свойстве: JET_SPACEHINTS. Улгровс'
title: Свойство JET_SPACEHINTS. Улгровс
TOCTitle: 'ulGrowth property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.JET_SPACEHINTS.ulGrowth
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.jet_spacehints.ulgrowth(v=EXCHG.10)
ms:contentKeyID: 55103929
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.JET_SPACEHINTS.ulGrowth
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.JET_SPACEHINTS.set_ulGrowth
- Microsoft.Isam.Esent.Interop.JET_SPACEHINTS.ulGrowth
- Microsoft.Isam.Esent.Interop.JET_SPACEHINTS.get_ulGrowth
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 293450e968092443021817037c0da1bde3c4e04870dfa0eee4ae9bcb3deea2af
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120016444"
---
# <a name="jet_spacehintsulgrowth-property"></a>Свойство JET_SPACEHINTS. Улгровс

Возвращает или задает процент роста по отношению к последнему или исходному размеру (возможно, округленному до ближайшего размера выделенной памяти JET). Допустимые значения: 0, \[ 100, 50000).

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Property ulGrowth As Integer
    Get
    Set
'Usage
Dim instance As JET_SPACEHINTS
Dim value As Integer

value = instance.ulGrowth

instance.ulGrowth = value
```

``` csharp
public int ulGrowth { get; set; }
```

#### <a name="property-value"></a>Значение свойства

Тип: [System. Int32](/dotnet/api/system.int32)  

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Справочник

[Класс JET_SPACEHINTS](./jet-spacehints-class.md)

[Элементы JET_SPACEHINTS](./jet-spacehints-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
