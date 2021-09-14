---
title: Перечисление MPTHREAT_SEVERITY (Мпклиент. h)
description: Возможные угрозы угроз.
ms.assetid: 7C50AC74-16CB-4198-ABB2-D6999429F2EA
keywords:
- MPTHREAT_SEVERITY перечисления устаревших Windows компонентов среды
- PMPTHREAT_SEVERITYные компоненты среды Windows указателя перечисления
topic_type:
- apiref
api_name:
- MPTHREAT_SEVERITY
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2eec7bff3b23a89ce8187798d8a69a9968cbc2bf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241249"
---
# <a name="mpthreat_severity-enumeration"></a>\_Перечисление серьезности мпсреат

Возможные угрозы угроз.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum tagMPTHREAT_SEVERITY { 
  MP_THREAT_SEVERITY_UNKNOWN   = 0,
  MP_THREAT_SEVERITY_LOW       = 1,
  MP_THREAT_SEVERITY_MODERATE  = 2,
  MP_THREAT_SEVERITY_HIGH      = 4,
  MP_THREAT_SEVERITY_SEVERE    = 5,
  MP_THREAT_SEVERITY_MAXVALUE  = 5
} MPTHREAT_SEVERITY, *PMPTHREAT_SEVERITY;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="MP_THREAT_SEVERITY_UNKNOWN"></span><span id="mp_threat_severity_unknown"></span>**\_ \_ степень серьезности угрозы пакета управления \_ неизвестна**
</dt> <dd></dd> <dt>

<span id="MP_THREAT_SEVERITY_LOW"></span><span id="mp_threat_severity_low"></span>**\_ \_ низкий уровень серьезности угрозы пакета управления \_**
</dt> <dd></dd> <dt>

<span id="MP_THREAT_SEVERITY_MODERATE"></span><span id="mp_threat_severity_moderate"></span>**\_серьезность угрозы пакета управления — \_ \_ умеренный**
</dt> <dd></dd> <dt>

<span id="MP_THREAT_SEVERITY_HIGH"></span><span id="mp_threat_severity_high"></span>**\_ \_ высокий уровень серьезности угрозы пакета управления \_**
</dt> <dd></dd> <dt>

<span id="MP_THREAT_SEVERITY_SEVERE"></span><span id="mp_threat_severity_severe"></span>**\_серьезность угрозы пакета управления — \_ \_ серьезная**
</dt> <dd></dd> <dt>

<span id="MP_THREAT_SEVERITY_MAXVALUE"></span><span id="mp_threat_severity_maxvalue"></span>**\_ \_ степень серьезности угрозы пакета управления \_ MaxValue**
</dt> <dd></dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





