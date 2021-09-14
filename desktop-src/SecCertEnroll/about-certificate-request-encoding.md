---
description: В PKI Майкрософт запросы на сертификаты отправляются с клиентских компьютеров в центры сертификации (CAs) в виде двоичной строки, содержащей последовательность закодированных структур данных.
ms.assetid: 0b9fa1bc-b67e-4b50-abd5-cbc3663ff219
title: Кодирование запроса сертификата
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3cd9dfedede4c7b10d4968242b1d27ad11e2b6f0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173348"
---
# <a name="certificate-request-encoding"></a>Кодирование запроса сертификата

В PKI Майкрософт запросы на сертификаты отправляются с клиентских компьютеров в центры сертификации (CAs) в виде двоичной строки, содержащей последовательность закодированных структур данных. API регистрации сертификатов использует синтаксическую нотацию (ASN. 1) для описания и кодирования этих структур. Для целей этой документации ASN. 1 можно разделить на синтаксические правила (ISO 8824), описывающие структуры данных, и правила кодирования (ISO 8825), которые определяют способ кодирования данных для передачи по сети. Дополнительные сведения см. в следующих разделах:

-   [Общие сведения о синтаксисе и кодировке ASN. 1](about-introduction-to-asn-1-syntax-and-encoding.md)
-   [Система типов ASN. 1](about-asn-1-type-system.md)
-   [Distinguished Encoding Rules](distinguished-encoding-rules.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сведения об API регистрации сертификатов](about-the-certificate-enrollment-api.md)
</dt> </dl>

 

 



