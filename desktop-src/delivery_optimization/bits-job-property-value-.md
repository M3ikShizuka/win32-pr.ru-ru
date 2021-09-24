---
title: Структура BITS_JOB_PROPERTY_VALUE (Deliveryoptimization. h)
description: BITS_JOB_PROPERTY_VALUE Union предоставляет значение свойства задания оптимизации доставки на основе значения перечисления BITS_JOB_PROPERTY_ID.
ms.assetid: C24D9EA1-2E72-4403-939A-7B01D7133FE7
keywords:
- Структура BITS_JOB_PROPERTY_VALUE
- Структура BITS_JOB_PROPERTY_VALUE
topic_type:
- apiref
api_name:
- BITS_JOB_PROPERTY_VALUE
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 187026bf80638d1139e84e014b4f4de5d8d5d50d
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520552"
---
# <a name="bits_job_property_value-structure"></a>Структура BITS_JOB_PROPERTY_VALUE

**BITS_JOB_PROPERTY_VALUE** Union предоставляет значение свойства задания оптимизации доставки на основе значения перечисления [**BITS_JOB_PROPERTY_ID**](bits-job-property-id.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD          Dword;
  GUID           ClsID;
  BOOL           Enable;
  UINT64         Uint64;
  BG_AUTH_TARGET Target;
} BITS_JOB_PROPERTY_VALUE;
```



## <a name="members"></a>Участники

<dl> <dt>

**DWORD**
</dt> <dd>

Это значение возвращается при использовании идентификатора свойства Enum **BITS_JOB_PROPERTY_ID_COST_FLAGS** и применяется в качестве [политики передачи](https://www.bing.com/search?q=transfer+policy) в задании оптимизации доставки.

</dd> <dt>

**Этому**
</dt> <dd>

Это значение возвращается при использовании идентификатора свойства Enum **BITS_JOB_PROPERTY_NOTIFICATION_CLSID** и представляет CLSID объекта обратного вызова для регистрации в задании оптимизации доставки.

</dd> <dt>

**Включить**
</dt> <dd>

Не поддерживается.

</dd> <dt>

**UInt64**
</dt> <dd>

Не поддерживается.

</dd> <dt>

**Целевой объект**
</dt> <dd>

Не поддерживается.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**BITS_JOB_PROPERTY_ID**](bits-job-property-id.md)
</dt> <dt>

[**BITS_JOB_TRANSFER_POLICY**](bits-job-transfer-policy-.md)
</dt> </dl>

 

 





