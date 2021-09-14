---
title: Структура WINBIO_ANTI_SPOOF_POLICY (Винбио \_ types. h)
description: Представляет политику антиподмены для пользователя.
ms.assetid: 2B433AE8-21A0-4AF1-853C-9074527DB2E4
keywords:
- API структуры WINBIO_ANTI_SPOOF_POLICY биометрическая платформа Windows
- PWINBIO_ANTI_SPOOF_POLICY API биометрическая платформа Windows указателя структуры
topic_type:
- apiref
api_name:
- WINBIO_ANTI_SPOOF_POLICY
api_location:
- winbio_types.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3da8b7811afb1de1ad464675125f125ef0ceab73
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064633"
---
# <a name="winbio_anti_spoof_policy-structure"></a>\_ \_ Структура политики антифишинга винбио \_

Представляет политику антиподмены для пользователя.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _WINBIO_ANTI_SPOOF_POLICY {
  WINBIO_ANTI_SPOOF_POLICY_ACTION Action;
  WINBIO_POLICY_SOURCE            Source;
} WINBIO_ANTI_SPOOF_POLICY, *PWINBIO_ANTI_SPOOF_POLICY;
```



## <a name="members"></a>Участники

<dl> <dt>

**Действие**
</dt> <dd>

Тип действия, выполняемого для политики антиподмены.

</dd> <dt>

**Источник**
</dt> <dd>

Источник политики антиподмены.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                                                                                              |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Винбио \_ types. h (включите винбио. h для клиентских приложений или винбио \_ Adapters. h для адаптеров).</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ \_ \_ действие политики АНТИфишинга винбио \_**](winbio-anti-spoof-policy-action.md)
</dt> <dt>

[**\_источник политики \_ винбио**](winbio-policy-source.md)
</dt> <dt>

[**\_асинхронный \_ результат винбио**](/windows/desktop/api/Winbio/ns-winbio-winbio_async_result)
</dt> <dt>

[**винбиожетпроперти**](/windows/desktop/api/Winbio/nf-winbio-winbiogetproperty)
</dt> <dt>

[**винбиосетпроперти**](/windows/desktop/api/winbio/nf-winbio-winbiosetproperty)
</dt> </dl>

 

 





