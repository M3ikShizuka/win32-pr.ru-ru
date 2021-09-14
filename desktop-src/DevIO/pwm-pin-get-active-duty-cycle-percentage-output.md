---
description: Содержит текущий процент циклов работоспособности для ПИН-кода или канала в контроллере широты импульсов.
ms.assetid: 09C0232A-DF5C-4A1C-8138-D3D65E45731B
title: Структура PWM_PIN_GET_ACTIVE_DUTY_CYCLE_PERCENTAGE_OUTPUT (широт. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PWM_PIN_GET_ACTIVE_DUTY_CYCLE_PERCENTAGE_OUTPUT
api_type:
- HeaderDef
api_location:
- Pwm.h
ms.openlocfilehash: 607fcb1ab429e7cbe9aee593f75d48f0f9d308bd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164323"
---
# <a name="pwm_pin_get_active_duty_cycle_percentage_output-structure"></a>Закрепление широтного импульса \_ \_ Получение \_ активной \_ \_ \_ процентной структуры циклов пошлины \_

\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском. Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно приведенных здесь сведений.\]

Содержит текущий процент циклов работоспособности для ПИН-кода или канала в контроллере широты импульсов.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PWM_PIN_GET_ACTIVE_DUTY_CYCLE_PERCENTAGE_OUTPUT {
  PWM_PERCENTAGE Percentage;
} PWM_PIN_GET_ACTIVE_DUTY_CYCLE_PERCENTAGE_OUTPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**Percentage**
</dt> <dd>

Текущий цикл обработки сигнала ШИРОТы в виде коэффициента ШИРОТы в \_ процентах (улонглонг).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                      |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                             |
| Минимальная версия КМДФ<br/>     | 1,19<br/>                                                                                  |
| Минимальная версия UMDF<br/>     | 2.19<br/>                                                                                  |
| Заголовок<br/>                   | <dl> <dt>Широт. h (включая широту. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IOCTL \_ широтного \_ ПИН-кода \_ Получение \_ активной \_ пошлины в \_ \_ процентах**](https://www.bing.com/search?q=**IOCTL\_PWM\_PIN\_GET\_ACTIVE\_DUTY\_CYCLE\_PERCENTAGE**)
</dt> </dl>

 

 




