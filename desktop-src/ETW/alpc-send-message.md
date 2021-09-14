---
description: Этот класс является классом типа событий для ALPC "Отправка сообщения о событиях". Следующий синтаксис упрощен из MOF-кода.
ms.assetid: 7f12259b-f737-4bef-9dea-2ffe3517e0da
title: Класс ALPC_Send_Message
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ALPC_Send_Message
- ALPC_Send_Message.MessageID
api_type:
- NA
api_location: ''
ms.openlocfilehash: c9437626341f0ac57136645d40a8389436e8af1a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055418"
---
# <a name="alpc_send_message-class"></a>ALPC. \_ Отправка \_ класса сообщения

Этот класс является классом типа событий для ALPC "Отправка сообщения о событиях".

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType(33), EventTypeName("ALPC-Send-Message")]
class ALPC_Send_Message : ALPC
{
  uint32 MessageID;
};
```

## <a name="members"></a>Участники

Класс **\_ \_ сообщения ALPC Send** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **\_ \_ сообщения ALPC Send** имеет следующие свойства.

<dl> <dt>

**MessageID**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Идентификатор сообщения.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




