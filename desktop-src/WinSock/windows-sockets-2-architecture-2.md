---
description: архитектура Windows sockets 2 (Winsock) соответствует Windows архитектуре Open System (воса).
ms.assetid: d4cf1462-2e83-49a5-b698-350ff37aa497
title: Windows Архитектура сокетов 2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4ae85ad58a4206d75144e47662bd563fb3235eb1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967293"
---
# <a name="windows-sockets-2-architecture"></a>Windows Архитектура сокетов 2

архитектура Windows sockets 2 соответствует Windows архитектуре Open System (воса), как показано ниже:

![Архитектура Windows Sockets 2](images/ovrvw2-1.png)

Winsock определяет стандартный интерфейс поставщика услуг (SPI) между прикладным программным интерфейсом (API) и его функциями, экспортированными из WS2 \_32.dll и стеками протоколов. следовательно, поддержка Winsock не ограничена протоколами TCP/IP, как в случае с Windows сокетами 1,1.

архитектура Windows sockets 2 не является обязательной или желательной, чтобы поставщики стеков предWS2и собственную реализацию \_32.dll, так как одна WS2ная \_32.dll должна работать во всех стеках. WS2 \_32.dll и оболочки совместимости должны быть просмотрены так же, как компонент операционной системы.

 

 



