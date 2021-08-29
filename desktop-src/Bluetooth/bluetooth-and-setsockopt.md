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
ms.openlocfilehash: 70aef0914e13888f3bcb48bed5c7c90cd2585a5d22d60c27a35af605657f20c6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120004444"
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

 

 