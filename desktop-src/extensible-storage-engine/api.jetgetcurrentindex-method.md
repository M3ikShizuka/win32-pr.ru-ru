---
description: Дополнительные сведения о методе API. Жетжеткуррентиндекс
title: API. Жетжеткуррентиндекс, метод
TOCTitle: 'JetGetCurrentIndex method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Api.JetGetCurrentIndex(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID,System.String@,System.Int32)
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.api.jetgetcurrentindex(v=EXCHG.10)
ms:contentKeyID: 55100699
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Api.JetGetCurrentIndex
dev_langs:
- CSharp
- JScript
- VB
- other
api_name:
- Microsoft.Isam.Esent.Interop.Api.JetGetCurrentIndex
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: bacc6973b1a105e128533a1116abdeb4c6cfafa4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567127"
---
# <a name="apijetgetcurrentindex-method"></a>API. Жетжеткуррентиндекс, метод

Ддетерминес имя текущего индекса данного курсора. Это имя также используется для повторного выбора этого индекса в качестве текущего индекса с помощью [жетсеткуррентиндекс (JET_SESID, JET_TABLEID, String)](./api.jetsetcurrentindex-method.md). Его также можно использовать для обнаружения свойств этого индекса с помощью Жетжеттаблеиндексинфо.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Shared Sub JetGetCurrentIndex ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID, _
    <OutAttribute> ByRef indexName As String, _
    maxNameLength As Integer _
)
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim indexName As String
Dim maxNameLength As IntegerApi.JetGetCurrentIndex(sesid, tableid, _
    indexName, maxNameLength)
```

``` csharp
public static void JetGetCurrentIndex(
    JET_SESID sesid,
    JET_TABLEID tableid,
    out string indexName,
    int maxNameLength
)
```

#### <a name="parameters"></a>Параметры

  - сесид  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_SESID](./jet-sesid-structure.md)  
    
    Используемый сеанс.

<!-- end list -->

  - TableID  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_TABLEID](./jet-tableid-structure.md)  
    
    Курсор, для которого необходимо получить имя индекса.

<!-- end list -->

  - indexName  
    Тип: [System. String](/dotnet/api/system.string)  
    
    Возвращает имя индекса.

<!-- end list -->

  - maxNameLength  
    Тип: [System. Int32](/dotnet/api/system.int32)  
    
    Максимальная длина имени индекса. Длина имен индексов не превышает [намемост](./systemparameters.namemost-field.md) символов.

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Ссылка

[Класс API](./api-class.md)

[Члены API](./api-members.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
