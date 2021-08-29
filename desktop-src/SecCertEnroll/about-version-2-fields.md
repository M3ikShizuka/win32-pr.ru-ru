---
description: Сертификат X.509 версии 2 содержит основные поля, определенные в версии 1, а также следующие поля.
ms.assetid: 533d43d7-0c49-4461-8ba8-368c103feb4f
title: Поля версии 2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8f7aed470acfbc3c9a648de46f89a72dc3de361e61eed39cdce4aebbf28e133f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118903430"
---
# <a name="version-2-fields"></a>Поля версии 2

Сертификат X.509 версии 2 содержит основные поля, определенные в версии 1, а также следующие поля.

## <a name="issuer-unique-identifier"></a>Уникальный идентификатор поставщика

Содержит уникальное значение, которое может быть использовано для того, чтобы имя ЦС по стандарту X.500 однозначно идентифицировало этот ЦС при последующем многократном использовании различными объектами.

``` syntax
---------------------------------------------------------------------
-- Issuer Unique identifier
---------------------------------------------------------------------
issuerUniqueIdentifier ::= [1] IMPLICIT UniqueIdentifier OPTIONAL

UniqueIdentifier ::= BITSTRING
```

## <a name="subject-unique-identifier"></a>Уникальный идентификатор субъекта

Содержит уникальное значение, которое может быть использовано для того, чтобы имя субъекта по стандарту X.500 однозначно идентифицировало этот субъект при последующем многократном использовании различными объектами.

``` syntax
---------------------------------------------------------------------
-- Issuer Unique identifier
---------------------------------------------------------------------
subjectUniqueIdentifier ::= [2] IMPLICIT UniqueIdentifier OPTIONAL

UniqueIdentifier ::= BITSTRING
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Основные поля](about-basic-fields.md)
</dt> <dt>

[Расширения версии 3](about-version-3-extensions.md)
</dt> <dt>

[Сертификаты открытого ключа X. 509](about-x-509-public-key-certificates.md)
</dt> </dl>

 

 



