---
title: Структура MPHEALTH_DATA (Мпклиент. h)
description: Данные уведомления о работоспособности.
ms.assetid: 37A87F77-386A-4508-B338-ED2151518968
keywords:
- MPHEALTH_DATA структуры устаревшие функции среды Windows
- функции PMPHEALTH_DATA Windows указателя структур в устаревшей среде
topic_type:
- apiref
api_name:
- MPHEALTH_DATA
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e729bdea82b6a885b64e95ecd77f9deae6bff4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344423"
---
# <a name="mphealth_data-structure"></a>\_Структура данных мфеалс

Данные уведомления о работоспособности.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMPHEALTH_DATA {
  DWORD dwNotificationType;
  DWORD dwNotificationFlag;
} MPHEALTH_DATA, *PMPHEALTH_DATA;
```



## <a name="members"></a>Участники

<dl> <dt>

**двнотификатионтипе**
</dt> <dd>

Тип: **DWORD**

</dd> <dd>

Тип уведомления.

</dd> <dt>

**двнотификатионфлаг**
</dt> <dd>

Тип: **DWORD**

</dd> <dd>

Не используется.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





