---
title: Перечисление MPDETECTION_STATE (Мпклиент. h)
description: Состояние обнаруженной в настоящее время угрозы.
ms.assetid: 293771FF-A210-41D0-88A5-3B52ACAA9295
keywords:
- MPDETECTION_STATE перечисления устаревших Windows компонентов среды
- PMPDETECTION_STATEные компоненты среды Windows указателя перечисления
topic_type:
- apiref
api_name:
- MPDETECTION_STATE
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f9265a15641d2072d87b33af2782f17974bf07be
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252583"
---
# <a name="mpdetection_state-enumeration"></a>\_Перечисление состояний мпдетектион

Состояние обнаруженной в настоящее время угрозы.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum tagMPDETECTION_STATE { 
  MPDETECTION_STATE_UNKNOWN             = 0,
  MPDETECTION_STATE_ACTIVE              = 1,
  MPDETECTION_STATE_FINISHED            = 2,
  MPDETECTION_STATE_ADDITIONAL_ACTIONS  = 3,
  MPDETECTION_STATE_FAILED              = 4,
  MPDETECTION_STATE_CRITICALLY_FAILED   = 5,
  MPDETECTION_STATE_CLEARED             = 6
} MPDETECTION_STATE, *PMPDETECTION_STATE;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="MPDETECTION_STATE_UNKNOWN"></span><span id="mpdetection_state_unknown"></span>**\_Неизвестное состояние мпдетектион \_**
</dt> <dd>

В состоянии ошибки.

</dd> <dt>

<span id="MPDETECTION_STATE_ACTIVE"></span><span id="mpdetection_state_active"></span>**\_активное состояние \_ мпдетектион**
</dt> <dd>

Активная угроза.

</dd> <dt>

<span id="MPDETECTION_STATE_FINISHED"></span><span id="mpdetection_state_finished"></span>**\_состояние мпдетектион \_ завершено**
</dt> <dd>

Перемещение в незавершенное время в течение 24 часов.

</dd> <dt>

<span id="MPDETECTION_STATE_ADDITIONAL_ACTIONS"></span><span id="mpdetection_state_additional_actions"></span>**\_ \_ Дополнительные действия для состояния мпдетектион \_**
</dt> <dd>

Требуются дополнительные действия.

</dd> <dt>

<span id="MPDETECTION_STATE_FAILED"></span><span id="mpdetection_state_failed"></span>**\_Сбой состояния \_ мпдетектион**
</dt> <dd>

Некритическая ошибка исправления.

</dd> <dt>

<span id="MPDETECTION_STATE_CRITICALLY_FAILED"></span><span id="mpdetection_state_critically_failed"></span>**\_ \_ критический сбой состояния \_ мпдетектион**
</dt> <dd>

Критическая ошибка исправления.

</dd> <dt>

<span id="MPDETECTION_STATE_CLEARED"></span><span id="mpdetection_state_cleared"></span>**МПДЕТЕКТИОН \_ состояние \_ очистки**
</dt> <dd>

Угроза не отображается в запросе состояния, только в журнале.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



 

 





