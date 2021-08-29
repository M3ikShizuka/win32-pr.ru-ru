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
ms.openlocfilehash: 353faa17a505742f9e5b31feeb1c0108add7895f8039f12905c399d515bb2bb0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119910874"
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



## <a name="members"></a>Члены

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



 

 




