---
description: '\_Тип ПЕРЕЧИСЛЕНИЯ SMS Message Types \_ описывает тип содержимого сообщения SMS.'
ms.assetid: 882886a6-ecce-443f-a7e9-2e4e367ad804
title: Перечисление SMS_MESSAGE_TYPES (Портабледевице. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SMS_MESSAGE_TYPES
api_type:
- HeaderDef
api_location:
- PortableDevice.h
ms.openlocfilehash: a5b4ba0504f5407a49c04f84dd2ea3e152ee4de7bd78948a69046f257437eb75
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120006224"
---
# <a name="sms_message_types-enumeration"></a>\_ \_ Перечисление типов сообщений SMS

Тип **перечисления \_ SMS \_ Message** Types описывает тип содержимого сообщения SMS.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum SMS_MESSAGE_TYPES { 
  SMS_TEXT_MESSAGE    = 0,
  SMS_BINARY_MESSAGE  = 1
} ;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="SMS_TEXT_MESSAGE"></span><span id="sms_text_message"></span>**SMS \_ Text \_ Message**
</dt> <dd>

Текстовое сообщение.

</dd> <dt>

<span id="SMS_BINARY_MESSAGE"></span><span id="sms_binary_message"></span>**\_двоичное \_ сообщение SMS**
</dt> <dd>

Двоичное сообщение.

</dd> </dl>

## <a name="remarks"></a>Remarks

Это перечисление используется [**командой "WPD" \_ \_ SMS \_ Send**](wpd-command-sms-send-command.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Портабледевице. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Структуры и типы перечислений**](structures-and-enumeration-types.md)
</dt> </dl>

 

 




