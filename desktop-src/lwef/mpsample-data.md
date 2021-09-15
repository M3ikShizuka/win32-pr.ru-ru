---
title: Структура MPSAMPLE_DATA (Мпклиент. h)
description: Данные уведомления передаются в функцию обратного вызова отправки образца.
ms.assetid: 58F348C6-411D-4545-9D4D-A80095FD139B
keywords:
- MPSAMPLE_DATA структуры устаревшие функции среды Windows
- функции PMPSAMPLE_DATA Windows указателя структур в устаревшей среде
topic_type:
- apiref
api_name:
- MPSAMPLE_DATA
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 24a894638465c0362069b8fdcbacddf98bfdd2c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458819"
---
# <a name="mpsample_data-structure"></a>\_Структура данных мпсампле

Данные уведомления передаются в функцию обратного вызова отправки образца.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMPSAMPLE_DATA {
  DWORD dwSampleIndex;
} MPSAMPLE_DATA, *PMPSAMPLE_DATA;
```



## <a name="members"></a>Участники

<dl> <dt>

**двсамплеиндекс**
</dt> <dd>

Тип: **DWORD**

</dd> <dd>

Индекс образца элемента, для которого сообщается состояние отправки.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





