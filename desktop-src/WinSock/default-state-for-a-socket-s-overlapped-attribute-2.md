---
description: функция сокета создала сокеты с атрибутом overlapped, установленным по умолчанию в первой Wsock32.dll, 32-разрядной версией Windows сокетов 1,1.
ms.assetid: 2ebf71fd-fcb3-4f2f-bf52-14cd13af012f
title: Состояние по умолчанию для перекрывающихся атрибутов сокета
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ae64f5ba1481c62faf0798fa45aafdd98dde0696dfde68f79132d533ec3abce0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119860934"
---
# <a name="default-state-for-a-sockets-overlapped-attribute"></a>Состояние по умолчанию для перекрывающихся атрибутов сокета

функция [**сокета**](/windows/desktop/api/Winsock2/nf-winsock2-socket) создала сокеты с атрибутом overlapped, установленным по умолчанию в первой Wsock32.dll, 32-разрядной версией Windows сокетов 1,1. чтобы обеспечить обратную совместимость с развернутыми Wsock32.dll реализациями, это будет продолжаться и для Windows сокетов 2. то есть в сокетах сокетов Windows 2, созданных с помощью функции **сокета** , будет атрибут overlapped. однако, чтобы обеспечить более эффективную совместимость с остальной частью API Windows, сокеты, созданные с помощью [**всасоккет**](/windows/desktop/api/Winsock2/nf-winsock2-wsasocketa) , по умолчанию не будут иметь атрибут overlapped. Этот атрибут будет применен только в том случае, \_ Если \_ установлен бит с перекрытием флага WSA.

 

 



