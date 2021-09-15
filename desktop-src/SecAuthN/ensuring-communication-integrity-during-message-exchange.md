---
description: После установки контекста безопасности приложение может использовать функции поддержки сообщений для передачи сообщений, защищенных от изменения.
ms.assetid: 43d7b940-1816-429f-be6e-40978efed278
title: Обеспечение целостности связи во время Exchange сообщений
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 70545abf11a933cd3bb6d0c32f3312637fcccbe2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127271456"
---
# <a name="ensuring-communication-integrity-during-message-exchange"></a>Обеспечение целостности связи во время Exchange сообщений

После установки [*контекста безопасности*](/windows/desktop/SecGloss/s-gly) приложение может использовать функции [поддержки сообщений](authentication-functions.md) для передачи сообщений, защищенных от изменения.

Клиент или сервер передает контекст безопасности и сообщение в функцию [**макесигнатуре**](/windows/desktop/api/Sspi/nf-sspi-makesignature) для создания безопасной подписи, которая предотвращает изменение сообщения во время передачи. Получатель сообщения вызывает функцию [**VerifySignature**](/windows/desktop/api/Sspi/nf-sspi-verifysignature) . **VerifySignature** использует сведения в сигнатуре для проверки того, что полученное сообщение не было изменено во время передачи. Клиент и сервер могут также обмениваться зашифрованными сообщениями с помощью [**енкриптмессаже (General)**](/windows/win32/api/sspi/nf-sspi-encryptmessage) и [**декриптмессаже (General)**](/windows/win32/api/sspi/nf-sspi-decryptmessage).

Сервер в соединении с проверкой подлинности также может устанавливать соединения с другими удаленными компьютерами в имени клиента после вызова [**имперсонатесекуритиконтекст**](/windows/desktop/api/Sspi/nf-sspi-impersonatesecuritycontext).

 

 
