---
description: Net.exe можно использовать для завершения и запуска протокола IPv6.
ms.assetid: faa555d9-eb20-4b7a-94eb-b67a48ee630e
title: Net.exe
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5074696b71ce000ef330f2c88fceef0f60b0222e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249367"
---
# <a name="netexe"></a>Net.exe

Net.exe можно использовать для завершения и запуска протокола IPv6. Перезапуск IPv6 повторно инициализирует протокол, как если бы компьютер перезапускался, что может изменить номера интерфейсов. Net.exe имеет много подкоманд. Следующие команды относятся к протоколу IPv6:

<dl> <dt>

<span id="net_stop_tcpip6"></span><span id="NET_STOP_TCPIP6"></span>**NET tcpip6**
</dt> <dd>

Останавливает протокол IPv6 и выгружает его из памяти. Эта команда завершается ошибкой, если открыты какие-либо сокеты IPv6.

</dd> <dt>

<span id="net_start_tcpip6"></span><span id="NET_START_TCPIP6"></span>**NET start tcpip6**
</dt> <dd>

Запускает протокол IPv6, если он был остановлен. Если в каталоге% SystemRoot% System32 имеется новый файл драйвера Tcpip6.sys \\ , он \\ загружается.

</dd> </dl>

 

 



