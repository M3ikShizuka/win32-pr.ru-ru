---
description: Каждое свойство управления регистрацией сертификатов доступно для чтения и записи и имеет инициализированное значение по умолчанию, а также набор допустимых значений.
ms.assetid: e31dd6df-bc2a-401f-9343-a7dbb0f374bb
title: Использование свойств управления регистрацией сертификатов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4a556af6b75fe23e25efb3dcd4a6863a80592637921f6851f855aa8abccf5786
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118896643"
---
# <a name="using-the-certificate-enrollment-control-properties"></a>Использование свойств управления регистрацией сертификатов

Каждое свойство управления регистрацией сертификатов доступно для чтения и записи и имеет инициализированное значение по умолчанию, а также набор допустимых значений. Можно задать для свойства любое значение в этом наборе, чтобы изменить поведение методов, использующих свойство. Чтобы получить требуемое поведение, задайте свойство перед вызовом метода, который использует значение этого свойства.

Однако обратите внимание, что после вызова следующих методов

-   [**acceptPKCS7**](/windows/desktop/api/Xenroll/nf-xenroll-icenroll-acceptpkcs7)
-   [**acceptFilePKCS7**](/windows/desktop/api/Xenroll/nf-xenroll-icenroll-acceptfilepkcs7)
-   [**createPKCS10**](/windows/desktop/api/Xenroll/nf-xenroll-icenroll-createpkcs10)
-   [**createFilePKCS10**](/windows/desktop/api/Xenroll/nf-xenroll-icenroll-createfilepkcs10)

Сброс следующих свойств заблокирован

-   [**ProviderType**](/windows/win32/api/xenroll/nf-xenroll-icenroll-get_providertype)
-   [**KeySpec**](/windows/win32/api/xenroll/nf-xenroll-icenroll-get_keyspec)
-   [**провидерфлагс**](/windows/win32/api/xenroll/nf-xenroll-icenroll-get_providerflags)
-   [**ContainerName;**](/windows/win32/api/xenroll/nf-xenroll-icenroll-get_containername)
-   [**ProviderName**](/windows/win32/api/xenroll/nf-xenroll-icenroll-get_providername)

Если не вызывается метод [**ICEnroll4:: Reset**](/windows/desktop/api/Xenroll/nf-xenroll-icenroll3-reset) .

Сведения об отдельных свойствах и методах см. в справочных разделах, посвященных этим свойствам и методам в [справочнике по шифрованию](cryptography-reference.md).

В следующих разделах содержатся сведения, относящиеся к языку, для настройки и получения свойств управления регистрацией сертификатов.

-   [Свойства управления регистрацией сертификатов в C++](certificate-enrollment-control-properties-in-c-.md)

 

 
