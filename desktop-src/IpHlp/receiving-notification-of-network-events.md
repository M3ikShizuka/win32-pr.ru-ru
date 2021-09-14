---
description: Используйте следующие функции, чтобы убедиться, что приложение получает уведомления о некоторых сетевых событиях.
ms.assetid: e1ca5abf-83c2-44f0-8049-ddf1b81ef088
title: Получение уведомлений о сетевых событиях
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ecb9840f7ddf4adbfaae5775de337da81a3e7670
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144810"
---
# <a name="receiving-notification-of-network-events"></a>Получение уведомлений о сетевых событиях

Используйте следующие функции, чтобы убедиться, что приложение получает уведомления о некоторых сетевых событиях.

Используйте функцию [**нотифяддрчанже**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-notifyaddrchange) для запроса уведомления об изменениях, происходящих в сопоставлении между IP-адресами и интерфейсами на локальном компьютере.

Аналогичным образом функция [**нотифираутечанже**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-notifyroutechange) позволяет приложению запрашивать уведомления о любых изменениях, происходящих в таблице маршрутизации IP.

Уведомления, предоставляемые этими функциями, не указывают, что изменилось; они просто указывают, что что-то изменилось. Используйте другие вспомогательные функции IP, такие как [**жетипаддртабле**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-getipaddrtable) и [**жетбестрауте**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-getbestroute), чтобы определить точную природу изменения.

 

 



