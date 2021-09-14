---
description: Структура ПРОТОКОЛТАБЛЕ содержит список протоколов.
ms.assetid: dad2b228-5916-44fe-b78e-ebc6507dc555
title: Структура ПРОТОКОЛТАБЛЕ (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PROTOCOLTABLE
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: 3ad79beca7ce79611747a02704ffc05da5fc3d4b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348511"
---
# <a name="protocoltable-structure"></a>Структура ПРОТОКОЛТАБЛЕ

Структура **протоколтабле** содержит список протоколов.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PROTOCOLTABLE {
  DWORD     nProtocols;
  HPROTOCOL hProtocol[1];
} PROTOCOLTABLE;
```



## <a name="members"></a>Участники

<dl> <dt>

**нпротоколс**
</dt> <dd>

Число включенных протоколов.

</dd> <dt>

**хпротокол**
</dt> <dd>

Массив дескрипторов для включенных протоколов.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



 

 




