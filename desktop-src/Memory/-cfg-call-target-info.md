---
description: представляет сведения о целевых объектах вызова для управления Flow Guard (CFG).
ms.assetid: 8DEF907F-3F23-4122-95CE-F413FC7FD96B
title: Структура CFG_CALL_TARGET_INFO (Нтммапи. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CFG_CALL_TARGET_INFO
api_type:
- HeaderDef
api_location:
- ntmmapi.h
ms.openlocfilehash: 66177f6b478264a10c1ce0e50297d943a16407c4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144482"
---
# <a name="cfg_call_target_info-structure"></a>\_ \_ \_ Структура сведений о цели вызова cfg

представляет сведения о целевых объектах вызова для управления Flow Guard (CFG).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _CFG_CALL_TARGET_INFO {
  ULONG_PTR Offset;
  ULONG_PTR Flags;
} CFG_CALL_TARGET_INFO, *PCFG_CALL_TARGET_INFO;
```



## <a name="members"></a>Участники

<dl> <dt>

**Offset**
</dt> <dd>

Смещение относительно указанного (начального) виртуального адреса. Это смещение должно быть равно 16 байтам.

</dd> <dt>

**Флаги**
</dt> <dd>

Флаги, описывающие операцию, которая должна быть выполнена с адресом. Если задана **\_ \_ \_ допустимая цель вызова cfg** , адрес будет ПОМЕЧЕН как допустимый для cfg. В противном случае он будет помечен как недопустимый целевой объект вызова.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Нтммапи. h</dt> </dl> |



 

 




