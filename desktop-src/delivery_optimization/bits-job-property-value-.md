---
title: Структура BITS_JOB_PROPERTY_VALUE (Deliveryoptimization. h)
description: BITS_JOB_PROPERTY_VALUE Union предоставляет значение свойства задания DO на основе значения перечисления BITS_JOB_PROPERTY_ID.
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
ms.openlocfilehash: c48c1fe550db51b6b838379d44df21c95fa95e41
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567162"
---
# <a name="bits_job_property_value-structure"></a>Структура BITS_JOB_PROPERTY_VALUE

**BITS_JOB_PROPERTY_VALUE** Union предоставляет значение свойства задания Do на основе значения перечисления [**BITS_JOB_PROPERTY_ID**](bits-job-property-id.md) .

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

Это значение возвращается при использовании идентификатора свойства Enum **BITS_JOB_PROPERTY_ID_COST_FLAGS** и применяется в качестве [политики перемещения](https://www.bing.com/search?q=transfer+policy) в задании Do.

</dd> <dt>

**Этому**
</dt> <dd>

Это значение возвращается при использовании идентификатора свойства перечисления **BITS_JOB_PROPERTY_NOTIFICATION_CLSID** и представляет идентификатор CLSID объекта обратного вызова, регистрируемого в задании Do.

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

 

 





