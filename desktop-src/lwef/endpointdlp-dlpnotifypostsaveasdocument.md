---
description: Предоставляет системе сведения о документе после завершения операции Сохранить как.
title: Функция DlpNotifyPostSaveAsDocument (endpointdlp.h)
ms.topic: reference
ms.date: 03/18/2021
topic_type:
- APIRef
- kbSyntax
api_name:
- DlpNotifyPostSaveAsDocument
api_type:
- DllExport
api_location:
- EndpointDlp.dll
ms.openlocfilehash: ebdf21bd4d4d212c66ae54c4439e30b9efbf91b9c7ffeb1d3edef0b6e8efdc3e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119962754"
---
# <a name="dlpnotifypostsaveasdocument-function"></a>Функция Длпнотифипостсавеасдокумент

Предоставляет системе сведения о документе после завершения операции Сохранить как.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI DlpNotifyPostSaveAsDocument(_In_ const PDLP_DOCUMENT_INFO DocumentInfo, _In_ LPCWSTR Destination, _In_ const PDLP_POSTOP_STATUS OpStatus); 
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*Документинфо* \[ окне\]
</dt> <dd>

Указатель на структуру [PDLP_DOCUMENT_INFO](endpointdlp-dlp_document_info.md) , содержащую сведения о сохраненном документе.

</dd> </dl>

<dl> <dt>

*Назначение* \[ окне\]
</dt> <dd>

Объект **лпквстр** , содержащий целевой путь к сохраненному документу.

</dd> </dl>

<dl> <dt>

*Опстатус* \[ окне\]
</dt> <dd>

Указатель на структуру [DLP_POSTOP_STATUS](enpointdlp-dlp_postop_status.md) , содержащую сведения о состоянии операции "Сохранить как".

</dd> </dl>


## <a name="return-value"></a>Возвращаемое значение

Возвращает значение void.

## <a name="remarks"></a>Remarks


## <a name="requirements"></a>Требования



| Требование          |    Значение                   |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, версия 1809 (10,0; Сборка 17763)           |
| DLL<br/>                      | EndpointDlp.dll |