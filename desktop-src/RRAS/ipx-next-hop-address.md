---
title: Структура IPX_NEXT_HOP_ADDRESS (RTM. h)
description: '\_ \_ Структура адреса следующего прыжка IPX \_ содержит адрес маршрутизатора следующего прыжка для IPX-маршрута.'
ms.assetid: 079e3284-6238-4bcf-a17f-68ff86775f18
keywords:
- RAS структуры IPX_NEXT_HOP_ADDRESS
- RAS — указатель структуры PIPX_NEXT_HOP_ADDRESS
topic_type:
- apiref
api_name:
- IPX_NEXT_HOP_ADDRESS
api_location:
- Rtm.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 99c3eb135f1d87050cd190fe47d0088fd1ab86f6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253699"
---
# <a name="ipx_next_hop_address-structure"></a>\_ \_ Структура адреса следующего ПРЫЖКа IPX \_

\[этот api был заменен api [диспетчера таблиц маршрутизации версии 2](about-routing-table-manager-version-2.md) и не будет доступен за пределами Windows Server 2003. Приложения должны использовать API диспетчера таблиц маршрутизации версии 2.\]

Структура **\_ \_ \_ адреса следующего прыжка IPX** содержит адрес маршрутизатора следующего прыжка для IPX-маршрута.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _IPX_NEXT_HOP_ADDRESS {
  BYTE NHA_Mac[6];
} IPX_NEXT_HOP_ADDRESS, *PIPX_NEXT_HOP_ADDRESS;
```



## <a name="members"></a>Участники

<dl> <dt>

**НХА \_ Mac**
</dt> <dd>

Указывает MAC-адрес маршрутизатора следующего прыжка.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                        |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                   |
| Заголовок<br/>                   | <dl> <dt>RTM. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Справочник по диспетчеру таблиц маршрутизации версии 1](routing-table-manager-version-1-reference.md)
</dt> <dt>

[Структуры диспетчера таблиц маршрутизации версии 1](routing-table-manager-version-1-structures.md)
</dt> <dt>

[**\_маршрут IPX \_ RTM**](rtm-ipx-route.md)
</dt> </dl>

 

 





