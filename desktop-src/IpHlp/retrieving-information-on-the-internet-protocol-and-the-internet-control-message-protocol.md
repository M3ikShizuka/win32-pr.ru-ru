---
description: Вспомогательная служба IP предоставляет возможности извлечения данных, которые полезны для сетевого администрирования локального компьютера.
ms.assetid: b50b3927-6c74-4282-b79b-c86d72d93ae3
title: Получение сведений о протоколе Интернета и протоколе управляющих сообщений Интернета
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9b5d009ea045e66a65cf585b2196c56ea13ea95c14938b838d1572c9d563a303
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119897814"
---
# <a name="retrieving-information-on-the-internet-protocol-and-the-internet-control-message-protocol"></a>Получение сведений о протоколе Интернета и протоколе управляющих сообщений Интернета

Вспомогательная служба IP предоставляет возможности извлечения данных, которые полезны для сетевого администрирования локального компьютера. Следующие функции извлекают статистику по протоколу IP и ICMP. Эти функции также можно использовать для задания определенных параметров конфигурации для IP.

Функция [**жетипстатистикс**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-getipstatistics) извлекает текущую статистику IP-адресов для локального компьютера. Примеры кода, включающие **жетипстатистикс** , см. [в разделе Получение сведений с помощью жетипстатистикс](retrieving-information-using-getipstatistics.md).

Функция [**жетикмпстатистикс**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-geticmpstatistics) извлекает текущую статистику ICMP.

Используйте функцию [**сетипстатистикс**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-setipstatistics) для включения или отключения IP-пересылки. Эта функция также дает возможность задать срок жизни (TTL) по умолчанию для IP-датаграмм. Кроме того, можно задать TTL с помощью функции [**сетипттл**](/windows/desktop/api/Iphlpapi/nf-iphlpapi-setipttl) .

 

 



