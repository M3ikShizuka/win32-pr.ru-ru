---
description: 'Дополнительные сведения: метод API. Макекэй (JET_SESID, JET_TABLEID, Int16, Макекэйгрбит)'
title: Метод API. Макекэй (JET_SESID, JET_TABLEID, Int16, Макекэйгрбит)
TOCTitle: MakeKey method (JET_SESID, JET_TABLEID, Int16, MakeKeyGrbit)
ms:assetid: M:Microsoft.Isam.Esent.Interop.Api.MakeKey(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID,System.Int16,Microsoft.Isam.Esent.Interop.MakeKeyGrbit)
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.api.makekey(v=EXCHG.10)
ms:contentKeyID: 55100840
ms.date: 07/30/2014
ms.topic: reference
dev_langs:
- vb
- csharp
api_name:
- Microsoft.Isam.Esent.Interop.Api.MakeKey
topic_type:
- apiref
- kbSyntax
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 485d79851dc25c0370e5c1f92ca0da19eae3a2fb7c0e2263b987bc535f0f5214
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120067134"
---
# <a name="apimakekey-method-jet_sesid-jet_tableid-int16-makekeygrbit"></a>Метод API. Макекэй (JET_SESID, JET_TABLEID, Int16, Макекэйгрбит)

Конструирует ключ поиска, который затем может использоваться [жетсик (JET_SESID, JET_TABLEID, сикгрбит)](./api.jetseek-method.md) и [жетсетиндексранже (JET_SESID, JET_TABLEID, сетиндексранжегрбит)](./api.jetsetindexrange-method.md).

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Shared Sub MakeKey ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID, _
    data As Short, _
    grbit As MakeKeyGrbit _
)
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim data As Short
Dim grbit As MakeKeyGrbitApi.MakeKey(sesid, tableid, data, _
    grbit)
```

``` csharp
public static void MakeKey(
    JET_SESID sesid,
    JET_TABLEID tableid,
    short data,
    MakeKeyGrbit grbit
)
```

#### <a name="parameters"></a>Параметры

  - сесид  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_SESID](./jet-sesid-structure.md)  
    
    Используемый сеанс.

<!-- end list -->

  - TableID  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_TABLEID](./jet-tableid-structure.md)  
    
    Курсор, на котором создается ключ.

<!-- end list -->

  - .  
    Тип: [System. Int16](/dotnet/api/system.int16)  
    
    Данные столбца для текущего ключевого столбца текущего индекса.

<!-- end list -->

  - грбит  
    Тип: [Microsoft. ISAM. ESENT. Interop. макекэйгрбит](./makekeygrbit-enumeration.md)  
    
    Ключевые параметры.

## <a name="see-also"></a>См. также

#### <a name="reference"></a>Справочник

[Класс API](./api-class.md)

[Члены API](./api-members.md)

[Перегрузка Макекэй](./api.makekey-method.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
