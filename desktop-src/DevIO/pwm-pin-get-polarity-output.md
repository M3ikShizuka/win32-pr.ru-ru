---
description: Содержит значение полярности для возврата.
ms.assetid: 432C10EF-AC08-4781-9BCA-A31E0DF12704
title: Структура PWM_PIN_GET_POLARITY_OUTPUT (широт. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PWM_PIN_GET_POLARITY_OUTPUT
api_type:
- HeaderDef
api_location:
- Pwm.h
ms.openlocfilehash: 81cf7b658a0024c3280db1523af34aaf2ef17262
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164320"
---
# <a name="pwm_pin_get_polarity_output-structure"></a>\_Схема \_ \_ \_ вывода данных о полярности с модулятором

\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском. Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно приведенных здесь сведений.\]

Содержит значение полярности для возврата.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PWM_PIN_GET_POLARITY_OUTPUT {
  PWM_POLARITY Polarity;
} PWM_PIN_GET_POLARITY_OUTPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**Полярность**
</dt> <dd>

Полярность ПИН-кода или канала в виде значения [**\_ полярности широты**](/windows/desktop/api/Pwm/ne-pwm-pwm_polarity) . Значение полярности — "активный" или "низкий".

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

[**IOCTL \_ широтного \_ ПИН-кода \_ Получение \_ полярности**](https://www.bing.com/search?q=**IOCTL\_PWM\_PIN\_GET\_POLARITY**)
</dt> <dt>

[**\_полярность широты**](/windows/win32/api/pwm/ne-pwm-pwm_polarity)
</dt> </dl>

 

