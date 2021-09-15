---
title: 'Авторизация службы '
description: Приложение может реализовать пользовательскую авторизацию для входящих сообщений на узле службы.
ms.assetid: 75bcf051-3983-48fc-8121-0984ac9cdcb9
keywords:
- Веб-службы авторизации служб для Windows
- ввсапи
- WWS
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c296dc6b4900bd20df7d1e70631e758599a0028d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574218"
---
# <a name="service-authorization"></a>Авторизация службы 

Приложение может реализовать пользовательскую авторизацию для входящих сообщений на узле службы.


Узел службы получает [**\_ \_ \_ обратный вызов безопасности службы**](/windows/desktop/api/WebServices/nc-webservices-ws_service_security_callback) обратного вызова WS в рамках [**\_ \_ конечной точки службы WS**](/windows/desktop/api/WebServices/ns-webservices-ws_service_endpoint) , который передается функции [**WsCreateServiceHost**](/windows/desktop/api/WebServices/nf-webservices-wscreateservicehost) . Этот обратный вызов вызывается при получении [ \_ сообщения WS](ws-message.md) .

Приложение может полагаться на этот обратный вызов, чтобы реализовать пользовательскую авторизацию для входящих сообщений на узле службы. Если авторизация не удалась, функция обратного вызова безопасности возвращает кадр сбоя, а узел службы прерывает канал.

Пример реализации см. в примере имени пользователя через SSL example, [хттпкалкулаторвисусернамеоверсслсервицеексампле](httpcalculatorwithusernameoversslserviceexample.md).

 

 




