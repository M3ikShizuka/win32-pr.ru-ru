---
description: 'Дополнительные сведения о свойстве: JET_RETRIEVECOLUMN. cbData'
title: Свойство JET_RETRIEVECOLUMN. cbData
TOCTitle: 'cbData property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.JET_RETRIEVECOLUMN.cbData
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.jet_retrievecolumn.cbdata(v=EXCHG.10)
ms:contentKeyID: 55103810
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.JET_RETRIEVECOLUMN.cbData
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.JET_RETRIEVECOLUMN.set_cbData
- Microsoft.Isam.Esent.Interop.JET_RETRIEVECOLUMN.get_cbData
- Microsoft.Isam.Esent.Interop.JET_RETRIEVECOLUMN.cbData
topic_type:
- apiref
- kbSyntax
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 8012a305fef042e27749be233741b2cf85acd0994a9164c553e374e3e966a7c9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119038692"
---
# <a name="jet_retrievecolumncbdata-property"></a>Свойство JET_RETRIEVECOLUMN. cbData

Возвращает или задает размер буфера [пвдата](./jet-retrievecolumn.pvdata-property.md) в байтах. Операция получения столбца не будет хранить больше данных в Пвдата, чем cbData.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Property cbData As Integer
    Get
    Set
'Usage
Dim instance As JET_RETRIEVECOLUMN
Dim value As Integer

value = instance.cbData

instance.cbData = value
```

``` csharp
public int cbData { get; set; }
```

#### <a name="property-value"></a>Значение свойства

Тип: [System. Int32](/dotnet/api/system.int32)  

## <a name="see-also"></a>См. также

#### <a name="reference"></a>Справочник

[Класс JET_RETRIEVECOLUMN](./jet-retrievecolumn-class.md)

[Элементы JET_RETRIEVECOLUMN](./jet-retrievecolumn-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
