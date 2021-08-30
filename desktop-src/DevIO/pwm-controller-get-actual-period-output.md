---
description: Содержит действующий период вывода сигнала для контроллера ШИРОТы импульсов.
ms.assetid: 280F564F-FF7F-4121-B726-9F9AF9E98EB7
title: Структура PWM_CONTROLLER_GET_ACTUAL_PERIOD_OUTPUT (широт. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PWM_CONTROLLER_GET_ACTUAL_PERIOD_OUTPUT
api_type:
- HeaderDef
api_location:
- Pwm.h
ms.openlocfilehash: 3f51f360e7b6ff3966ed58d8ec3a171d8bbbfb54672c50c31852e71ab6750f95
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120088144"
---
# <a name="pwm_controller_get_actual_period_output-structure"></a>Контроллер ШИРОТы \_ \_ получения \_ фактической \_ \_ структуры выходных данных периода

\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно предоставленной здесь информации.\]

Содержит действующий период вывода сигнала для контроллера ШИРОТы импульсов.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PWM_CONTROLLER_GET_ACTUAL_PERIOD_OUTPUT {
  PWM_PERIOD ActualPeriod;
} PWM_CONTROLLER_GET_ACTUAL_PERIOD_OUTPUT;
```



## <a name="members"></a>Члены

<dl> <dt>

**актуалпериод**
</dt> <dd>

Эффективный период вывода сигналов, который будет измеряться в выходных каналах контроллера.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                      |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                             |
| Минимальная версия КМДФ<br/>     | 1,19<br/>                                                                                  |
| Минимальная версия UMDF<br/>     | 2.19<br/>                                                                                  |
| Заголовок<br/>                   | <dl> <dt>Широт. h (включая широту. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_ \_ \_ \_ текущий период получения контроллера ШИРОТного модулятора ioctl \_**](https://www.bing.com/search?q=**IOCTL\_PWM\_CONTROLLER\_GET\_ACTUAL\_PERIOD**)
</dt> </dl>

 

 




