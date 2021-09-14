---
title: Bluetooth и сетсоккопт
description: Bluetooth использует функцию сетсоккопт для установки различных параметров, связанных с каналом сервера или соединением.
ms.assetid: ab78baed-5556-4d7b-88a6-e3ceb93afa8c
keywords:
- Bluetooth
- сетсоккопт
- Bluetooth и сетсоккопт
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 943839a49788b76e597596aee9cba65fa4b8d30d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172100"
---
# <a name="bluetooth-and-setsockopt"></a>Bluetooth и сетсоккопт

Bluetooth использует функцию [**сетсоккопт**](/windows/desktop/api/winsock/nf-winsock-setsockopt) для установки различных параметров, связанных с каналом сервера или соединением. использование **сетсоккопт** с Bluetooth имеет следующие требования.

-   параметр *s* параметра [**сетсоккопт**](/windows/desktop/api/winsock/nf-winsock-setsockopt) должен быть допустимым сокетом Bluetooth.
-   Параметр *Level* параметра [**СЕТСОККОПТ**](/windows/desktop/api/winsock/nf-winsock-setsockopt) должен быть Sol \_ RFCOMM.

список доступных параметров сокета Bluetooth см. в разделе [Bluetooth и параметры сокета](bluetooth-and-socket-options.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> <dt>

[**сетсоккопт**](/windows/desktop/api/winsock/nf-winsock-setsockopt)
</dt> </dl>

 

 