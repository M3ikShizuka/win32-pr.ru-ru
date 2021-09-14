---
title: Bluetooth и принять
description: Bluetooth использует функцию accept для включения входящих попыток подключения к сокету.
ms.assetid: 79708118-2f70-4759-b5d6-cf5cfc33c27e
keywords:
- accept
- Bluetooth
- Bluetooth
- Bluetooth и принять
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 28dff84ec05429411614e64a08ab159a5ee134b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973178"
---
# <a name="bluetooth-and-accept"></a>Bluetooth и принять

Bluetooth использует функцию [**accept**](/windows/desktop/api/winsock2/nf-winsock2-accept) для включения входящих попыток подключения к сокету. бс \_ -адрес клиентского приложения получается путем считывания Bluetooth относящегося к транспорту раздела возвращенной структуры [**sockaddr**](/windows/desktop/WinSock/sockaddr-2) . использование функции **accept** с Bluetooth имеет следующий формат:

-   Параметр *addr* функции [**Accept**](/windows/desktop/api/winsock2/nf-winsock2-accept) является необязательным указателем на буфер, который получает адрес связывающей сущности, как известно на уровне связи. возвращается указатель на структуру [**\_ бс SOCKADDR**](/windows/desktop/api/Ws2bth/ns-ws2bth-sockaddr_bth) с адресом удаленного Bluetooth устройства.
-   Параметр *аддрлен* функции [**Accept**](/windows/desktop/api/winsock2/nf-winsock2-accept) является необязательным указателем на целое число, которое содержит длину адреса в байтах. Целое число должно быть больше или равно значению **sizeof** ([**SOCKADDR \_ БС**](/windows/desktop/api/Ws2bth/ns-ws2bth-sockaddr_bth)).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> <dt>

[**гласит**](/windows/desktop/api/winsock2/nf-winsock2-accept)
</dt> </dl>

 

 