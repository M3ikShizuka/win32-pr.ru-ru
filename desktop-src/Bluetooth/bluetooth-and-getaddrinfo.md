---
title: Bluetooth и функцию getaddrinfo
description: Функция функцию getaddrinfo предоставляет преобразование из имени узла в адрес для транспортов на основе IP-адресов. поскольку функция функцию getaddrinfo относится только к транспортам на основе IP-адресов, она завершается сбоем на Bluetooth сокетах.
ms.assetid: e17d8542-d4bc-499c-bae4-1f41bff493c3
keywords:
- Bluetooth и функцию getaddrinfo Bluetooth
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 96c2e62b83ac947b74479ff435b93914661aa8da
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973165"
---
# <a name="bluetooth-and-getaddrinfo"></a>Bluetooth и функцию getaddrinfo

Функция [**функцию getaddrinfo**](/windows/desktop/api/ws2tcpip/nf-ws2tcpip-getaddrinfo) предоставляет преобразование из имени узла в адрес для транспортов на основе IP-адресов. поскольку функция **функцию getaddrinfo** относится только к транспортам на основе IP-адресов, она завершается сбоем на Bluetooth сокетах.

чтобы выполнить преобразование из имени узла в адрес для сокетов Bluetooth, используйте функцию [**всалукупсервицебегин**](bluetooth-and-wsalookupservicebegin-for-device-inquiry.md) с **\_ контейнерами луп** для запроса удаленных устройств, а затем найдите конкретное соответствующее удаленное имя и соответствующий адрес.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> <dt>

[**функцию getaddrinfo**](/windows/desktop/api/ws2tcpip/nf-ws2tcpip-getaddrinfo)
</dt> <dt>

[**всалукупсервицебегин**](/windows/desktop/api/winsock2/nf-winsock2-wsalookupservicebegina)
</dt> </dl>

 

 