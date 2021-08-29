---
description: 'Дополнительные сведения: метод API. Жетсетсистемпараметер (JET_INSTANCE, JET_SESID, JET_param, IntPtr, String)'
title: Метод API. Жетсетсистемпараметер (JET_INSTANCE, JET_SESID, JET_param, IntPtr, String)
TOCTitle: JetSetSystemParameter method (JET_INSTANCE, JET_SESID, JET_param, IntPtr, String)
ms:assetid: M:Microsoft.Isam.Esent.Interop.Api.JetSetSystemParameter(Microsoft.Isam.Esent.Interop.JET_INSTANCE,Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_param,System.IntPtr,System.String)
ms:mtpsurl: https://msdn.microsoft.com/library/microsoft.isam.esent.interop.api.jetsetsystemparameter(v=EXCHG.10)
ms:contentKeyID: 55100822
ms.date: 07/30/2014
ms.topic: reference
dev_langs:
- vb
- csharp
api_name:
- Microsoft.Isam.Esent.Interop.Api.JetSetSystemParameter
topic_type:
- kbSyntax
- apiref
api_type:
- Managed
api_location:
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 18790ad7fa550ad3cd9383de7bc5d0639c3bbf1ddb218152aa7e90dac3e6a411
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119977464"
---
# <a name="apijetsetsystemparameter-method-jet_instance-jet_sesid-jet_param-intptr-string"></a>Метод API. Жетсетсистемпараметер (JET_INSTANCE, JET_SESID, JET_param, IntPtr, String)

Задает параметры конфигурации базы данных.

**Пространство имен:**  [Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)  
**Сборка:**  Microsoft. ISAM. ESENT. Interop (в Microsoft.Isam.Esent.Interop.dll)

## <a name="syntax"></a>Синтаксис

``` vb
'Declaration
Public Shared Function JetSetSystemParameter ( _
    instance As JET_INSTANCE, _
    sesid As JET_SESID, _
    paramid As JET_param, _
    paramValue As IntPtr, _
    paramString As String _
) As JET_wrn
'Usage
Dim instance As JET_INSTANCE
Dim sesid As JET_SESID
Dim paramid As JET_param
Dim paramValue As IntPtr
Dim paramString As String
Dim returnValue As JET_wrn

returnValue = Api.JetSetSystemParameter(instance, _
    sesid, paramid, paramValue, paramString)
```

``` csharp
public static JET_wrn JetSetSystemParameter(
    JET_INSTANCE instance,
    JET_SESID sesid,
    JET_param paramid,
    IntPtr paramValue,
    string paramString
)
```

#### <a name="parameters"></a>Параметры

  - экземпляр  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_INSTANCE](./jet-instance-structure.md)  
    
    Экземпляр, устанавливающий параметр ON или [nil](./jet-instance.nil-property.md) , чтобы задать параметр для всех экземпляров.

<!-- end list -->

  - сесид  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_SESID](./jet-sesid-structure.md)  
    
    Используемый сеанс.

<!-- end list -->

  - paramid  
    Тип: [Microsoft.ISAM.ESENT.Interop.JET_param](./jet-param-enumeration.md)  
    
    Заданный параметр.

<!-- end list -->

  - paramValue  
    Тип: [System. IntPtr](/dotnet/api/system.intptr)  
    
    Значение параметра, которое необходимо задать, если параметр имеет целочисленный тип.

<!-- end list -->

  - парамстринг  
    Тип: [System. String](/dotnet/api/system.string)  
    
    Значение параметра, которое необходимо задать, если параметр имеет строковый тип.

#### <a name="return-value"></a>Возвращаемое значение

Тип: [Microsoft.ISAM.ESENT.Interop.JET_wrn](./jet-wrn-enumeration.md)  
Код предупреждения ESENT.  

## <a name="see-also"></a>См. также раздел

#### <a name="reference"></a>Справочник

[Класс API](./api-class.md)

[Члены API](./api-members.md)

[Перегрузка Жетсетсистемпараметер](./api.jetsetsystemparameter-method.md)

[Пространство имен Microsoft. ISAM. ESENT. Interop](./microsoft.isam.esent.interop-namespace.md)
