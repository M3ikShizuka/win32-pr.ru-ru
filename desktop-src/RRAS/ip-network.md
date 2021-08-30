---
title: Структура IP_NETWORK (RTM. h)
description: Структура IP- \_ сети описывает IP-адрес сети.
ms.assetid: 5dcc733f-c86f-407e-8727-64f3ae71dd48
keywords:
- RAS структуры IP_NETWORK
- RAS — указатель структуры PIP_NETWORK
topic_type:
- apiref
api_name:
- IP_NETWORK
api_location:
- Rtm.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5976211d0aea5936278353a9fb1b172585c0ee63531dde229ef4bf561c5dbb4e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120029964"
---
# <a name="ip_network-structure"></a>Структура IP- \_ сети

\[этот api был заменен api [диспетчера таблиц маршрутизации версии 2](about-routing-table-manager-version-2.md) и не будет доступен за пределами Windows Server 2003. Приложения должны использовать API диспетчера таблиц маршрутизации версии 2.\]

Структура **IP- \_ сети** описывает IP-адрес сети.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _IP_NETWORK {
  DWORD N_NetNumber;
  DWORD N_NetMask;
} IP_NETWORK, *PIP_NETWORK;
```



## <a name="members"></a>Члены

<dl> <dt>

**N \_ нетнумбер**
</dt> <dd>

Указывает номер IP-сети, выраженный в виде IP-адреса в порядке байтов на компьютере.

</dd> <dt>

**N \_ Маска сети**
</dt> <dd>

Указывает маску сети. Примените эту маску к IP-адресу, чтобы извлечь сетевой адрес. Маска сети находится в порядке байтов на уровне компьютера.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                        |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                   |
| Заголовок<br/>                   | <dl> <dt>RTM. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Справочник по диспетчеру таблиц маршрутизации версии 1](routing-table-manager-version-1-reference.md)
</dt> <dt>

[Структуры диспетчера таблиц маршрутизации версии 1](routing-table-manager-version-1-structures.md)
</dt> <dt>

[**Окончательная версия \_ IP- \_ маршрута**](rtm-ip-route.md)
</dt> </dl>

 

 





