---
title: Bluetooth и всасетсервице
description: Bluetooth использует функцию всасетсервице для регистрации или удаления экземпляра службы в пространстве имен Bluetooth (NS \_ бс) из реестра.
ms.assetid: 71c5ed9c-fade-4d15-848e-eb810ad4cbb2
keywords:
- Bluetooth Bluetooth
- Всасетсервице Bluetooth
- Bluetooth и всасетсервице Bluetooth
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 70399b73bf24477ee1a0ec0c7585a9f46b7657ef
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127261899"
---
# <a name="bluetooth-and-wsasetservice"></a>Bluetooth и всасетсервице

Bluetooth использует функцию [**всасетсервице**](/windows/desktop/api/winsock2/nf-winsock2-wsasetservicea) для регистрации или удаления экземпляра службы в пространстве имен Bluetooth (NS \_ бс) из реестра. Маркер, возвращаемый этой операцией, может использоваться только для удаления службы.

в Bluetooth есть два средства объявления служб с помощью функции [**всасетсервице**](/windows/desktop/api/winsock2/nf-winsock2-wsasetservicea) :

-   в приложении может быть объявлена простая запись службы Bluetooth SDP, созданная на основе стандартных членов в структуре [**всакуерисет**](/windows/desktop/api/winsock2/ns-winsock2-wsaquerysetw) .
-   приложение может объявить собственную запись SDP Bluetooth, передав структуру [**\_ \_ службы бс SET**](/windows/desktop/api/Ws2bth/ns-ws2bth-bth_set_service) в элемент **лпблоб** структуры [**всакуерисет**](/windows/desktop/api/winsock2/ns-winsock2-wsaquerysetw) . Это более сложный подход.

> [!Note]  
> Записи SDP, объявленные [**всасетсервице**](/windows/desktop/api/winsock2/nf-winsock2-wsasetservicea) , не сохраняются после завершения процесса, который их опубликовал.

 

использование [**всасетсервице**](/windows/desktop/api/winsock2/nf-winsock2-wsasetservicea) с Bluetooth имеет следующие требования.

-   Параметр *лпксрегинфо* — это адрес структуры [**всакуерисет**](/windows/desktop/api/winsock2/ns-winsock2-wsaquerysetw) , подрегистрируемой.
-   Параметр *ессоператион* является перечислением, которое содержит одну из операций, показанных в следующей таблице.



| Значение                  | Описание                                                                                |
|------------------------|--------------------------------------------------------------------------------------------|
| РНРСЕРВИЦЕ \_ регистр   | начинает объявлять службу для запросов удаленных радиостанций с помощью протокола Bluetooth SDP. |
| РНРСЕРВИЦЕ \_ Отмена регистрации | Недопустимый. Возвращает ошибку.                                                               |
| РНРСЕРВИЦЕ \_ Удаление     | Останавливает объявление службы.                                                             |



 

> [!Note]  
> Дескрипторы служб, обнаруженные во время вызова [**всалукупсервицебегин**](/windows/desktop/api/winsock2/nf-winsock2-wsalookupservicebegina) или [**всалукупсервиценекст**](/windows/desktop/api/winsock2/nf-winsock2-wsalookupservicenexta) , несовместимы с \_ операцией удаления рнрсервице.

 

-   Параметр *двконтролфлагс* зарезервирован и должен быть равен нулю.

дополнительные сведения и список параметров сокетов Bluetooth см. в разделе [Bluetooth и параметры сокета](bluetooth-and-socket-options.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сокеты Windows](/windows/desktop/WinSock/windows-sockets-start-page-2)
</dt> </dl>

 

 