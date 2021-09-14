---
title: Bluetooth и сокет
description: Создает сокет для входящих или исходящих соединений.
ms.assetid: 21b9cf1f-1a85-4a4b-9557-faa4f32c3696
keywords:
- Bluetooth Bluetooth
- Bluetooth сокета
- Bluetooth Bluetooth и сокетов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3c2c2085ee0c61941bab93ed25dd86f5c102d0d0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172096"
---
# <a name="bluetooth-and-socket"></a>Bluetooth и сокет

Функция [**Socket**](/windows/desktop/api/winsock2/nf-winsock2-socket) создает сокет для входящих или исходящих соединений.

чтобы создать сокет с помощью Bluetooth, используйте следующие параметры:

-   параметр *af* функции [**socket**](/windows/desktop/api/winsock2/nf-winsock2-socket) всегда имеет значение **af \_ бс** для сокетов Bluetooth.
-   Параметр *типа* функции [**Socket**](/windows/desktop/api/winsock2/nf-winsock2-socket) всегда **Сокк \_ Stream**; **Сокк \_** Сокеты дграм не поддерживаются Bluetooth.
-   Для параметра *протокола* **бспрото \_ RFCOMM** является поддерживаемым протоколом.

дополнительные сведения см. в разделе [сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> <dt>

[**фиксатор**](/windows/desktop/api/winsock2/nf-winsock2-socket)
</dt> </dl>

 

 