---
description: В следующем коде показаны функции recv и Send, используемые сервером.
ms.assetid: 26990b06-196a-4fb1-92d8-c5fa096d2b09
title: Получение и отправка данных на сервере
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 31ab20f074db750bef6459c6b9fcb5fd5636a522
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458228"
---
# <a name="receiving-and-sending-data-on-the-server"></a>Получение и отправка данных на сервере

В следующем коде показаны функции [**recv**](/windows/desktop/api/winsock/nf-winsock-recv) и [**Send**](/windows/desktop/api/Winsock2/nf-winsock2-send) , используемые сервером.

### <a name="to-receive-and-send-data-on-a-socket"></a>Получение и отправка данных на сокете


```C++
#define DEFAULT_BUFLEN 512

char recvbuf[DEFAULT_BUFLEN];
int iResult, iSendResult;
int recvbuflen = DEFAULT_BUFLEN;

// Receive until the peer shuts down the connection
do {

    iResult = recv(ClientSocket, recvbuf, recvbuflen, 0);
    if (iResult > 0) {
        printf("Bytes received: %d\n", iResult);

        // Echo the buffer back to the sender
        iSendResult = send(ClientSocket, recvbuf, iResult, 0);
        if (iSendResult == SOCKET_ERROR) {
            printf("send failed: %d\n", WSAGetLastError());
            closesocket(ClientSocket);
            WSACleanup();
            return 1;
        }
        printf("Bytes sent: %d\n", iSendResult);
    } else if (iResult == 0)
        printf("Connection closing...\n");
    else {
        printf("recv failed: %d\n", WSAGetLastError());
        closesocket(ClientSocket);
        WSACleanup();
        return 1;
    }

} while (iResult > 0);
```



Функции [**Send**](/windows/desktop/api/Winsock2/nf-winsock2-send) и [**recv**](/windows/desktop/api/winsock/nf-winsock-recv) возвращают целочисленное значение числа отправленных или полученных байтов соответственно, или ошибка. Каждая функция также принимает одни и те же параметры: активный сокет, буфер **char** , число байтов для отправки или получения и любые используемые флаги.

Следующий шаг: [Отключение сервера](disconnecting-the-server.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[начало работы с помощью Winsock](getting-started-with-winsock.md)
</dt> <dt>

[Серверное приложение Winsock](winsock-server-application.md)
</dt> <dt>

[Принятие подключения](accepting-a-connection.md)
</dt> </dl>

 

 



