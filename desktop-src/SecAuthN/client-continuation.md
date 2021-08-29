---
description: Для некоторых протоколов требуется несколько сообщений проверки подлинности.
ms.assetid: b4c4c38c-0286-49b1-b93d-4c6b885fe0f6
title: Продолжение клиента
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 007a6fbc3d9fd887b041bf23267ddb804665d733e057c717041ae02b3bb53513
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119883454"
---
# <a name="client-continuation"></a>Продолжение клиента

Для некоторых протоколов требуется несколько сообщений проверки подлинности. В этом случае клиент анализирует ответ от сервера и вызывает [**InitializeSecurityContext (Общие)**](/windows/win32/api/sspi/nf-sspi-initializesecuritycontexta) еще раз, используя состояние continue из предыдущего вызова. Клиент проверяет состояние возврата с помощью этого вызова и может потребоваться для продолжения дополнительных отрезков. Он использует сведения в *паутпут* для создания сообщения и его отправки на сервер.

 

 
