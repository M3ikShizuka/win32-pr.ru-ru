---
description: Этот класс является классом типа событий для ALPC ожидание событий ответа. Следующий синтаксис упрощен из MOF-кода.
ms.assetid: 9aaa2c93-41cc-4025-80f9-b7740a37c4d8
title: Класс ALPC_Wait_For_Reply
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ALPC_Wait_For_Reply
- ALPC_Wait_For_Reply.MessageID
api_type:
- NA
api_location: ''
ms.openlocfilehash: 898077511db25ec7f53bc075ecb845d04e540626
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127274896"
---
# <a name="alpc_wait_for_reply-class"></a>ALPC. \_ Ожидание \_ \_ класса ответа

Этот класс является классом типа событий для ALPC ожидание событий ответа.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType(35), EventTypeName("ALPC-Wait-For-Reply")]
class ALPC_Wait_For_Reply : ALPC
{
  uint32 MessageID;
};
```

## <a name="members"></a>Участники

Классу « **\_ ожидание в классе \_ \_ ответов** » в ALPC имеются следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Эти свойства имеют класс **ALPC \_ Wait \_ для класса \_ Reply** .

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



 

 




