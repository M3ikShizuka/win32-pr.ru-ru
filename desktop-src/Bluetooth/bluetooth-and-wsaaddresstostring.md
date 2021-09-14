---
title: Bluetooth и всааддресстостринг
description: функция всааддресстостринг Windows sockets используется для преобразования адреса устройства Bluetooth в строку, которая, в свою очередь, предоставляется функции всалукупсервицебегин через структуру всакуерисет при получении сведений о службе устройства.
ms.assetid: 3489d29a-2b64-4051-b579-57878efc0c73
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a78e8a9ae3ea6a0f853619a3f3610a64204ad3c3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172091"
---
# <a name="bluetooth-and-wsaaddresstostring"></a>Bluetooth и всааддресстостринг

функция [**всааддресстостринг**](/windows/desktop/api/winsock2/nf-winsock2-wsaaddresstostringa) Windows sockets используется для преобразования адреса устройства Bluetooth в строку, которая, в свою очередь, предоставляется функции [**всалукупсервицебегин**](/windows/desktop/api/winsock2/nf-winsock2-wsalookupservicebegina) через структуру [**всакуерисет**](/windows/desktop/api/winsock2/ns-winsock2-wsaquerysetw) при получении сведений о службе устройства.

хотя адрес устройства Bluetooth помещается в 20-символьный буфер, функция [**всааддресстостринг**](/windows/desktop/api/winsock2/nf-winsock2-wsaaddresstostringa) в настоящее время возвращает **всаефаулт** для адресов устройств Bluetooth, если только буфер и указанное значение *лпдваддрессстрингленгс* не имеют символьную длину 40.

> [!Note]  
> Если [**всааддресстостринг**](/windows/desktop/api/winsock2/nf-winsock2-wsaaddresstostringa) возвращает **всаефаулт** в результате недостаточного буфера, параметр *лпдваддрессстрингленгс* не обновляется с учетом размера буфера, необходимого для операции.

 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**всааддресстостринг**](/windows/desktop/api/winsock2/nf-winsock2-wsaaddresstostringa)
</dt> <dt>

[Bluetooth и всалукупсервицебегин](bluetooth-and-wsalookupservicebegin.md)
</dt> <dt>

[Bluetooth и всакуерисет](bluetooth-and-wsaqueryset.md)
</dt> </dl>

 

 