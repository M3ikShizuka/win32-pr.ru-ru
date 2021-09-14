---
title: Bluetooth и bind
description: Bluetooth использует функцию bind для привязки к сокету.
ms.assetid: 308d2680-de51-49e6-a0da-7aba494d9572
keywords:
- bind
- Bluetooth
- Bluetooth
- Bluetooth и bind
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 12ccbd088ab61edcfa3dfc511ea591593d0cf781
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973177"
---
# <a name="bluetooth-and-bind"></a>Bluetooth и bind

Bluetooth использует функцию [**bind**](/windows/desktop/api/winsock/nf-winsock-bind) для привязки к сокету. чтобы привязать Bluetooth сокет, вызовите функцию **bind** с помощью [**структуры \_ бс SOCKADDR**](/windows/desktop/api/Ws2bth/ns-ws2bth-sockaddr_bth) . Используйте структуру **SOCKADDR \_ БС** со следующими параметрами:

``` syntax
name.addressFamily = AF_BTH;
name.btAddr = 0;
name.serviceClassId = GUID_NULL;
name.port = number of service channel, 0 or BT_PORT_ANY;
```

Для клиентских приложений элемент порта должен быть равен нулю, чтобы обеспечить назначение соответствующей локальной конечной точки. В серверных приложениях элемент порта должен быть допустимым номером порта или BT- \_ портом \_ ANY; порты, автоматически назначенные с помощью BT- \_ порта, \_ могут быть запрошены в дальнейшем при вызове функции [**жетсоккнаме**](bluetooth-and-getsockname.md) . Допустимый диапазон для запроса определенного порта RFCOMM — от 1 до 30. каналы сервера — это глобальный ресурс, и на любом Bluetooth устройстве доступно только 30 каналов сервера, которые должны быть общими для всех Windows сокетов, принадлежащих семейству адресов Bluetooth. Если канал сервера недоступен или указанный канал сервера уже зарезервирован, вызов [**привязки**](/windows/desktop/api/winsock/nf-winsock-bind) завершается ошибкой.

После успешного возврата из BIND канал сервера резервируется до закрытия сокета. Используйте функцию [**жетсоккнаме**](bluetooth-and-getsockname.md) , чтобы получить номер канала для регистрации SDP.

Приложения должны использовать автоматическое выделение для канала сервера.

функция [**bind**](/windows/desktop/api/winsock/nf-winsock-bind) не объявляет серверное приложение автоматически с помощью Bluetooth SDP; приложения должны вызывать функцию [**всасетсервице**](/windows/desktop/api/winsock2/nf-winsock2-wsasetservicea) для обнаружения удаленными приложениями Bluetooth.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> <dt>

[**выполняется**](/windows/desktop/api/winsock/nf-winsock-bind)
</dt> </dl>

 

 