---
title: Структура MPNIS_PRIVATE_DATA (Мпклиент. h)
description: Частные уведомления NIS.
ms.assetid: 19B4928F-BC78-4DEA-A563-1516B6454465
keywords:
- MPNIS_PRIVATE_DATA структуры устаревшие функции среды Windows
- функции PMPNIS_PRIVATE_DATA Windows указателя структур в устаревшей среде
topic_type:
- apiref
api_name:
- MPNIS_PRIVATE_DATA
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 21340665a32b619c42d7909e8cd1b72ca6d09fb7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572886"
---
# <a name="mpnis_private_data-structure"></a>\_Структура закрытых \_ данных мпнис

Частные уведомления NIS.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMPNIS_PRIVATE_DATA {
  DWORD dwNotificationType;
  DWORD cbDataSize;
  BYTE  *pbData;
} MPNIS_PRIVATE_DATA, *PMPNIS_PRIVATE_DATA;
```



## <a name="members"></a>Участники

<dl> <dt>

**двнотификатионтипе**
</dt> <dd>

Тип: **DWORD**

</dd> <dd>

Тип уведомления.

</dd> <dt>

**кбдатасизе**
</dt> <dd>

Тип: **DWORD**

</dd> <dd>

Размер зарезервированных данных в байтах.

</dd> <dt>

**pbData**
</dt> <dd>

Тип: **Byte \***

</dd> <dd>

Указатель на зарезервированные данные.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





