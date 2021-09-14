---
description: Содержит номер порта, используемый для протоколов IP или IPX.
ms.assetid: 730f6ee6-7b7d-4e10-91ee-a4ba87aae5aa
title: Объединение GENERIC_PORT (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GENERIC_PORT
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: 3b684ffea65e85854d2928931f492fb247cc0b70
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171488"
---
# <a name="generic_port-union"></a>УНИВЕРСАЛЬНое \_ объединение портов

**Универсальная структура \_ порта** содержит номер порта, используемый для протоколов IP или IPX.

## <a name="syntax"></a>Синтаксис


```C++
typedef union {
  BYTE IPPort;
  WORD ByteSwappedIPXPort;
} GENERIC_PORT;
```



## <a name="members"></a>Участники

<dl> <dt>

**иппорт**
</dt> <dd>

Номер IP-порта, введенный в.

</dd> <dt>

**битесваппедипкспорт**
</dt> <dd>

Номер порта IPX, введенный в.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



 

 




