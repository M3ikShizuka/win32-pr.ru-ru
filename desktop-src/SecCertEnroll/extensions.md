---
description: Формат сертификата X. 509 версии 3 определяет несколько расширений, которые могут быть добавлены к сертификату.
ms.assetid: f2a6854d-1831-489f-adf6-31a0b26511e3
title: Расширения (API регистрации сертификатов)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Extensions
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 5478b8edeff3524ada760cc5680f5c9dca359e7a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056997"
---
# <a name="extensions-certificate-enrollment-api"></a>Расширения (API регистрации сертификатов)

Формат сертификата X. 509 версии 3 определяет несколько расширений, которые могут быть добавлены к сертификату. Расширения предоставляют расширенные сведения об использовании ключа, политиках сертификатов и ограничениях, альтернативных формах имен и многом другом. Для определения значения расширения можно использовать интерфейс [**IX509Extension**](/windows/desktop/api/CertEnroll/nn-certenroll-ix509extension) . Многие из распространенных расширений можно создать с помощью стандартных интерфейсов, производных от **IX509Extension**. Коллекция расширений добавляется в запрос сертификата путем включения коллекции в атрибуты запроса. Дополнительные сведения см. в следующих разделах:

-   [Поддерживаемые расширения](supported-extensions.md)
-   [\#Расширения PKCS 10](pkcs--10-extensions.md)
-   [Расширения CMC](cmc-extensions.md)

 

 



