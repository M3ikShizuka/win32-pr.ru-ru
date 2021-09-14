---
title: Структура MPTHREAT_STATS (Мпклиент. h)
description: Статистика, связанная с угрозами.
ms.assetid: 78B7E2A8-1BB4-4610-8E90-1F8ECBE740A8
keywords:
- MPTHREAT_STATS структуры устаревшие функции среды Windows
- функции PMPTHREAT_STATS Windows указателя структур в устаревшей среде
topic_type:
- apiref
api_name:
- MPTHREAT_STATS
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 21a2eef7acde5fbeac2cf9951dfad3e6923ccea2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168296"
---
# <a name="mpthreat_stats-structure"></a>\_Структура статистики мпсреат

Статистика, связанная с угрозами.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMPTHREAT_STATS {
  UINT ThreatCount;
  UINT SuspiciousThreatCount;
  UINT Reserved[4];
} MPTHREAT_STATS, *PMPTHREAT_STATS;
```



## <a name="members"></a>Участники

<dl> <dt>

**среаткаунт**
</dt> <dd>

Тип: **uint**

</dd> <dd>

Число обнаруженных угроз.

</dd> <dt>

**суспиЦиауссреаткаунт**
</dt> <dd>

Тип: **uint**

</dd> <dd>

Число обнаруженных угроз с мониторингом поведения.

</dd> <dt>

**Reserved**
</dt> <dd>

Тип: **uint \[ 4 \]**

</dd> <dd>

Поля, зарезервированные для будущего использования.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





