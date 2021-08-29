---
description: Структура ПРОТОКОЛИНФО описывает протокол.
ms.assetid: 7f936c93-a942-4591-9abc-59872df0964e
title: Структура ПРОТОКОЛИНФО (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PROTOCOLINFO
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: d44bf19f651f9391dcfc872798f709c463a74ce22b328c6942a32ca1a98636a0
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119889763"
---
# <a name="protocolinfo-structure"></a>Структура ПРОТОКОЛИНФО

Структура **протоколинфо** описывает протокол.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PROTOCOLINFO {
  DWORD              ProtocolID;
  LPPROPERTYDATABASE PropertyDatabase;
  BYTE               ProtocolName[16];
  BYTE               HelpFile[16];
  BYTE               Comment[128];
} PROTOCOLINFO, *LPPROTOCOLINFO;
```



## <a name="members"></a>Члены

<dl> <dt>

**протоколид**
</dt> <dd>

Назначенный системой идентификатор протокола для указанного сеанса выполнения.

</dd> <dt>

**пропертидатабасе**
</dt> <dd>

База данных свойств указанного протокола.

</dd> <dt>

**ProtocolName**
</dt> <dd>

Сокращенное имя протокола.

</dd> <dt>

**HelpFile**
</dt> <dd>

Необязательное имя файла справки, связанное с протоколом.

</dd> <dt>

**Комментарий**
</dt> <dd>

Комментарий, описывающий протокол.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



 

 




