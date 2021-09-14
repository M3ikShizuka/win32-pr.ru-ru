---
description: После того как сервер завершит получение данных от клиента и отправит данные обратно клиенту, сервер отключится от клиента и завершит работу сокета.
ms.assetid: 67f33645-d57a-48bd-9f0c-9e816f528204
title: Отключение сервера
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a6abf7754da39a891b3d29c69f6c835706debd36
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056247"
---
# <a name="disconnecting-the-server"></a>Отключение сервера

После того как сервер завершит получение данных от клиента и отправит данные обратно клиенту, сервер отключится от клиента и завершит работу сокета.

**Отключение и завершение работы сокета**

1.  Когда сервер отправляет данные клиенту, функция [**завершения работы**](/windows/desktop/api/winsock/nf-winsock-shutdown) может быть вызвана указанием SD \_ Send для завершения отправной стороны сокета. Это позволяет клиенту освобождать некоторые ресурсы для этого сокета. Серверное приложение по-прежнему может принимать данные через сокет.
    ```C++
    // shutdown the send half of the connection since no more data will be sent
    iResult = shutdown(ClientSocket, SD_SEND);
    if (iResult == SOCKET_ERROR) {
        printf("shutdown failed: %d\n", WSAGetLastError());
        closesocket(ClientSocket);
        WSACleanup();
        return 1;
    }
    ```

    

2.  Когда клиентское приложение выполняет получение данных, вызывается функция [**функции closesocket**](/windows/desktop/api/winsock/nf-winsock-closesocket) для закрытия сокета.

    после завершения работы клиентского приложения с помощью библиотеки DLL Windows sockets функция [**всаклеануп**](/windows/desktop/api/winsock/nf-winsock-wsacleanup) вызывается для освобождения ресурсов.

    ```C++
    // cleanup
    closesocket(ClientSocket);
    WSACleanup();

    return 0;
    ```

    

## <a name="complete-server-source-code"></a>Полный исходный код сервера

-   [Полный код сервера](complete-server-code.md)

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[начало работы с помощью Winsock](getting-started-with-winsock.md)
</dt> <dt>

[Серверное приложение Winsock](winsock-server-application.md)
</dt> <dt>

[Получение и отправка данных на сервере](receiving-and-sending-data-on-the-server.md)
</dt> <dt>

[Выполнение примера кода клиента и сервера Winsock](finished-server-and-client-code.md)
</dt> </dl>

 

 



