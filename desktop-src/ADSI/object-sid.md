---
title: Идентификатор безопасности объекта (поставщик WinNT)
description: Идентификатор безопасности пользователя (SID) можно получить с помощью атрибута objectSID. ObjectSID возвращается в виде массива вариантов символов, образующих строку идентификатора безопасности.
ms.assetid: 15845e6d-ea30-4d6c-9f35-b2abc1a564ba
ms.tgt_platform: multiple
keywords:
- Службы WinNT Provider ADSI, примеры управления пользователями, идентификатор безопасности объекта
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8d5d47e939770b9584a85e4e628c5c168901fc1f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126887101"
---
# <a name="object-sid-winnt-provider"></a>Идентификатор безопасности объекта (поставщик WinNT)

Идентификатор безопасности пользователя (SID) можно получить с помощью атрибута **objectSid** . **ObjectSid** возвращается в виде массива **вариантов** символов, образующих строку идентификатора безопасности.

## <a name="example-code"></a>Пример кода


```VB
sid = usr.Get("objectSID")
For i = LBound(sid) To UBound(sid)
    Debug.Print sid(i)
Next
```



 

 




