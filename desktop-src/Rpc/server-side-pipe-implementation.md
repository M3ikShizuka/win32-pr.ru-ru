---
title: Реализация Server-Sideного канала
description: Серверным программам для распределенных приложений, использующих каналы, не требуется реализовывать какие-либо функции push, Pull или Alloc.
ms.assetid: de733075-5767-4d46-b294-089c7e3cc695
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6927350e10061850c5fac0ab0db7c18570dd2bab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461480"
---
# <a name="server-side-pipe-implementation"></a>Реализация Server-Sideного канала

Серверным программам для распределенных приложений, использующих каналы, не требуется реализовывать какие-либо функции push, Pull или Alloc. Они должны содержать процедуры, которые клиенты могут вызывать удаленно для инициации передачи данных. В следующих разделах в этом разделе объясняется, как можно реализовать удаленные процедуры на сервере.

-   [Реализация входных каналов на сервере](implementing-input-pipes-on-the-server.md)
-   [Реализация выходных каналов на сервере](implementing-output-pipes-on-the-server.md)

 

 




