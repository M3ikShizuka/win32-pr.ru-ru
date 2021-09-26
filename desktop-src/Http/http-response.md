---
title: HTTP_RESPONSE (HTTP. h)
description: Версия структуры HTTP\_RESPONSE зависит от версии очереди запросов, используемой HTTP Server API. Версия 1.0 использует структуру HTTP\_RESPONSE\_V1. Версия 2.0 использует структуру HTTP\_RESPONSE\_V2.
ms.assetid: F94646C0-7293-4543-842B-F08D8C7E2247
keywords:
- _HTTP_RESPONSE
- HTTP_RESPONSE
- PHTTP_RESPONSE
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4a8445021aa61b94ae83a55937b1db5ca4e3c577
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127266288"
---

# HTTP\_RESPONSE

Версия структуры **HTTP\_RESPONSE** зависит от версии очереди запросов, используемой следующим образом:

-   HTTP Server API Version 1.0: [**HTTP\_RESPONSE\_V1**](/windows/win32/api/http/ns-http-http_response_v1).
-   HTTP Server API Version 2.0: [**HTTP\_RESPONSE\_V2**](/windows/win32/api/http/ns-http-http_response_v2).

Не используйте [**HTTP\_RESPONSE\_V1**](/windows/win32/api/http/ns-http-http_response_v1) и [**HTTP\_RESPONSE\_V2**](/windows/win32/api/http/ns-http-http_response_v2) непосредственно в коде; использование **HTTP\_RESPONSE** гарантирует правильную версию структуры на основе версии очереди запросов.


```C++
typedef HTTP_RESPONSE_V1 HTTP_RESPONSE;
typedef HTTP_RESPONSE_V2 HTTP_RESPONSE;
typedef HTTP_RESPONSE* PHTTP_RESPONSE;
```



<dl> <dt>

**HTTP\_RESPONSE_V1**
</dt> <dd>

Запрос был получен из очереди запросов v1.

</dd> <dt>

**HTTP\_RESPONSE_V2**
</dt> <dd>

Запрос был получен из очереди запросов v2.

</dd> <dt>

**PHTTP\_RESPONSE**
</dt> <dd>

Указатель на структуру **HTTP\_RESPONSE** .

</dd> </dl>

## Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                    |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                              |
| Заголовок<br/>                   | <dl> <dt>HTTP. h</dt> </dl> |



 

 





