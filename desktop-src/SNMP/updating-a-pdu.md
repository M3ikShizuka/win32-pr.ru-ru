---
title: Обновление PDU
description: Приложение WinSNMP может извлекать и обновлять выбранные поля PDU с помощью функций Снмпжетпдудата и Снмпсетпдудата.
ms.assetid: 001f5252-aa54-490b-8ff0-39a7780baff8
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4c876f22118841b2139086665aa2f39c4dd5395328a27e21cea35cf609698f48
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119885694"
---
# <a name="updating-a-pdu"></a>Обновление PDU

Приложение WinSNMP может извлекать и обновлять выбранные поля PDU с помощью функций [**снмпжетпдудата**](/windows/desktop/api/Winsnmp/nf-winsnmp-snmpgetpdudata) и [**снмпсетпдудата**](/windows/desktop/api/Winsnmp/nf-winsnmp-snmpsetpdudata) .

Приложение может получить поля типа PDU, идентификатора запроса, состояния ошибки и индекса ошибок из определенного PDU. Он также может получить маркер для списка привязок переменных. Приложение может обновлять поля **\_ типа PDU** и **\_ идентификатора запроса** .

Если тип PDU равен числу PDU SNMP \_ \_ , то приложение также может обновлять **\_ неповторяющиеся** значения и поля **максимального числа \_ повторений** PDU.

 

 




