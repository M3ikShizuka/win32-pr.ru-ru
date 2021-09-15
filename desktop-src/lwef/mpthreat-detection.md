---
title: Перечисление MPTHREAT_DETECTION (Мпклиент. h)
description: Возможные известные неправильные типы обнаружения угроз.
ms.assetid: 14FCA9BD-A9A1-488B-B8E8-88DE0DF18F27
keywords:
- MPTHREAT_DETECTION перечисления устаревших Windows компонентов среды
- PMPTHREAT_DETECTIONные компоненты среды Windows указателя перечисления
topic_type:
- apiref
api_name:
- MPTHREAT_DETECTION
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 86edc0e1ca4ee130f2a2a4a678447771f1ae40ae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574991"
---
# <a name="mpthreat_detection-enumeration"></a>\_Перечисление мпсреат обнаружения

Возможные известные неправильные типы обнаружения угроз.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum tagMPTHREAT_DETECTION { 
  MP_THREAT_DETECTION_CONCRETE    = 0,
  MP_THREAT_DETECTION_HEURISTIC   = 1,
  MP_THREAT_DETECTION_GENERIC     = 2,
  MP_THREAT_DETECTION_SUSPICIOUS  = 4,
  MP_THREAT_DETECTION_FASTPATH    = 8
} MPTHREAT_DETECTION, *PMPTHREAT_DETECTION;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="MP_THREAT_DETECTION_CONCRETE"></span><span id="mp_threat_detection_concrete"></span>**\_ \_ конкретное обнаружение угроз MP \_**
</dt> <dd>

Обнаружена угроза через конкретные подписи.

</dd> <dt>

<span id="MP_THREAT_DETECTION_HEURISTIC"></span><span id="mp_threat_detection_heuristic"></span>**\_ \_ эвристика обнаружения угроз MP \_**
</dt> <dd>

Обнаружена угроза с помощью эвристического алгоритма.

</dd> <dt>

<span id="MP_THREAT_DETECTION_GENERIC"></span><span id="mp_threat_detection_generic"></span>**\_ \_ универсальное обнаружение угроз MP \_**
</dt> <dd>

Обнаружена угроза через универсальные подписи.

</dd> <dt>

<span id="MP_THREAT_DETECTION_SUSPICIOUS"></span><span id="mp_threat_detection_suspicious"></span>**\_обнаружение угроз с точки управления \_ \_**
</dt> <dd>

Обнаружена угроза с помощью функции мониторинга поведения.

</dd> <dt>

<span id="MP_THREAT_DETECTION_FASTPATH"></span><span id="mp_threat_detection_fastpath"></span>**\_ \_ фастпас обнаружения угроз \_ MP**
</dt> <dd>

Обнаружена угроза через фастпас.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





