---
description: Непрозрачный тип данных.
ms.assetid: 384dd6e0-726f-4100-a036-1cca6a332a64
title: PLSA_CLIENT_REQUEST (Нтсекпкг. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4a3685c3cd38843edfd4ae708a18761b6ee698c9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173379"
---
# <a name="plsa_client_request"></a>\_запрос клиента \_ плса

Тип **данных \_ \_ запроса клиента плса** является непрозрачным типом данных.

[*Локальный центр безопасности*](../secgloss/l-gly.md) (LSA) использует его для внутренних целей, чтобы поддерживать клиентскую информацию, относящуюся к отдельным запросам.


```C++
#include <windows.h>

typedef PVOID *PLSA_CLIENT_REQUEST;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Нтсекпкг. h</dt> </dl> |



 

 
