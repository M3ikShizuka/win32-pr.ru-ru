---
description: ниже приведено краткое справочное занятие по обеспечению безопасности Windows сокетов.
ms.assetid: 70210e86-ead6-4b0c-ae47-66b2ef0a8d11
title: Безопасное программирование Winsock
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a70d7a0710a4446486835ec14435fa7d7ba1458c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056216"
---
# <a name="secure-winsock-programming"></a>Безопасное программирование Winsock

ниже приведено краткое справочное занятие по обеспечению безопасности Windows сокетов. Он предназначен для понимания безопасности Winsock и вариантов, доступных разработчику защищенных сетевых приложений.

-   [Использование \_ реусеаддр и так далее \_ ексклусивеаддрусе](using-so-reuseaddr-and-so-exclusiveaddruse.md)
-   [Расширения безопасных сокетов Winsock](winsock-secure-socket-extensions.md)

Связь с помощью сокетов также может быть зашифрована с помощью стандартов SSL/TLS с помощью защищенного канала, также известного как технология SChannel. Schannel — это поставщик поддержки безопасности (SSP), который содержит набор протоколов безопасности, обеспечивающих проверку подлинности и безопасную закрытую связь с помощью шифрования. Schannel в основном используется для Интернет-приложений, требующих обмена данными по протоколу HTTP. Дополнительные сведения см. в разделе [безопасный канал](../secauthn/secure-channel.md).

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Secure Channel](../secauthn/secure-channel.md)
</dt> </dl>

 

 
