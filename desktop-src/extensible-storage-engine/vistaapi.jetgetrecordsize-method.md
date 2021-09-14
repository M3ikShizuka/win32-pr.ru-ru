---
description: 'Дополнительные сведения о методе: Вистаапи. Жетжетрекордсизе'
title: Вистаапи. Жетжетрекордсизе, метод (Microsoft. ISAM. ESENT. Interop. Vista)
TOCTitle: 'JetGetRecordSize method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetGetRecordSize(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID,Microsoft.Isam.Esent.Interop.Vista.JET_RECSIZE@,Microsoft.Isam.Esent.Interop.GetRecordSizeGrbit)
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.vista.vistaapi.jetgetrecordsize(v=EXCHG.10)
ms:contentKeyID: 55104285
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetGetRecordSize
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.Vista.VistaApi.JetGetRecordSize
topic_type:
- apiref
- kbSyntax
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 37576e39d83270dcac3333e4d1f78fce32bb2669
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126882605"
---
# <a name="vistaapijetgetrecordsize-method"></a>Вистаапи. Жетжетрекордсизе, метод

Извлекает сведения о размере записи из нужного расположения.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Shared Sub JetGetRecordSize ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID, _
    ByRef recsize As JET_RECSIZE, _
    grbit As GetRecordSizeGrbit _
)
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim recsize As JET_RECSIZE
Dim grbit As GetRecordSizeGrbitVistaApi.JetGetRecordSize(sesid, tableid, _
    recsize, grbit)
```

``` csharp
public static void JetGetRecordSize(
    JET_SESID sesid,
    JET_TABLEID tableid,
    ref JET_RECSIZE recsize,
    GetRecordSizeGrbit grbit
)
```

#### <a name="parameters"></a>Параметры

  - сесид  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_SESID](./jet-sesid-structure.md)  
    
    Используемый сеанс.

<!-- end list -->

  - TableID  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_TABLEID](./jet-tableid-structure.md)  
    
    Курсор, который будет использоваться для вызова API. Курсор должен быть размещен в записи или иметь подготовленное обновление.

<!-- end list -->

  - рексизе  
    Тип: [Microsoft.ISAM.ESENT.Interop.Vista.JET_RECSIZE](./jet-recsize-structure2.md)  
    
    Возвращает размер записи.

<!-- end list -->

  - грбит  
    Тип: [Microsoft. ISAM. ESENT. Interop. жетрекордсизегрбит](./getrecordsizegrbit-enumeration.md)  
    
    Параметры вызова.

## <a name="see-also"></a>См. также:

#### <a name="reference"></a>Справочник

[Класс Вистаапи](./vistaapi-class.md)

[Элементы Вистаапи](./vistaapi-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop. Vista](./microsoft.isam.esent.interop.vista-namespace.md)
