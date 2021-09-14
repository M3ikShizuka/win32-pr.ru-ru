---
description: Windows Сокеты 2 не предполагают, что сетевой порядок байтов для всех протоколов одинаков.
ms.assetid: 517c21b5-4b56-49f8-88ae-103fdfce6441
title: Расширенные подпрограммы преобразования Byte-Order
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9addb2b1527546b8a7d13eb90581a333f87c6f0e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056240"
---
# <a name="extended-byte-order-conversion-routines"></a>Расширенные подпрограммы преобразования Byte-Order

Windows Сокеты 2 не предполагают, что сетевой порядок байтов для всех протоколов одинаков. Для преобразования 16-разрядных и 32-разрядных количеств в байты и из сетевого порядка байтов предоставляется набор подпрограмм преобразования. Эти подпрограммы принимают в качестве входного параметра маркер сокета, имеющий связанную с ним структуру [**всапротокол \_ info**](/windows/win32/api/winsock2/ns-winsock2-wsaprotocol_infoa) . Элемент **нетворкбитеордер** структуры **\_ сведений о всапротокол** указывает нужный порядок байтов в сети (в настоящее время это либо с обратным порядком байтов, либо с прямым порядком байтов).

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**хтонл**](/windows/desktop/api/winsock/nf-winsock-htonl)
</dt> <dt>

[**хтонс**](/windows/desktop/api/winsock/nf-winsock-htons)
</dt> <dt>

[**нтохл**](/windows/desktop/api/winsock/nf-winsock-ntohl)
</dt> <dt>

[**нтохс**](/windows/desktop/api/winsock/nf-winsock-ntohs)
</dt> <dt>

[Перенос приложений сокета в Winsock](porting-socket-applications-to-winsock.md)
</dt> <dt>

[Вопросы программирования Winsock](winsock-programming-considerations.md)
</dt> <dt>

[**всахтонл**](/windows/desktop/api/Winsock2/nf-winsock2-wsahtonl)
</dt> <dt>

[**всахтонс**](/windows/desktop/api/Winsock2/nf-winsock2-wsahtons)
</dt> <dt>

[**всантохл**](/windows/desktop/api/Winsock2/nf-winsock2-wsantohl)
</dt> <dt>

[**всантохс**](/windows/desktop/api/Winsock2/nf-winsock2-wsantohs)
</dt> <dt>

[**\_сведения о всапротокол**](/windows/win32/api/winsock2/ns-winsock2-wsaprotocol_infoa)
</dt> </dl>

 

 
