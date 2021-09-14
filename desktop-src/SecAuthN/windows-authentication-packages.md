---
description: Windows пакеты аутентификации предоставляют службы проверки подлинности, реализуя зависящие от пакета функции для функций лсалогонусер и LsaCallAuthenticationPackage, предоставляемых LSA.
ms.assetid: 71f7eccd-694d-475f-b6d0-1eaf9ac468f5
title: Windows Пакеты проверки подлинности
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c4b14f74ad466e0010f7ab5ac766af908a7b4704
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146446"
---
# <a name="windows-authentication-packages"></a>Windows Пакеты проверки подлинности

Windows пакеты аутентификации предоставляют службы проверки подлинности, реализуя зависящие от пакета функции для функций [**лсалогонусер**](/windows/desktop/api/Ntsecapi/nf-ntsecapi-lsalogonuser) и [**LsaCallAuthenticationPackage**](/windows/desktop/api/Ntsecapi/nf-ntsecapi-lsacallauthenticationpackage) , предоставляемых LSA.

MSV1 \_ 0 является примером [*пакета проверки подлинности*](../secgloss/a-gly.md)Windows. Пакет MSV1 \_ 0 принимает имя пользователя и [*хэшированный*](../secgloss/h-gly.md) пароль, который выполняется в базе данных [*диспетчера учетных записей безопасности*](../secgloss/s-gly.md) (SAM). В зависимости от результатов поиска \_ пакет проверки подлинности MSV1 0 принимает или отклоняет попытки проверки подлинности.

список функций поддержки, предоставляемых LSA для использования Windows пакетах проверки подлинности, требующих системных служб, см. в разделе [функции LSA, вызываемые пакетами проверки подлинности](authentication-functions.md).

Windows пакеты проверки подлинности должны реализовывать набор функций, которые вызываются LSA. Полный список функций см. в разделе [функции, реализованные пакетами проверки подлинности](authentication-functions.md).

 

 
