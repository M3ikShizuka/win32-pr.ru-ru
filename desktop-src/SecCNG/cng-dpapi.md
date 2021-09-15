---
description: корпорация майкрософт предоставила интерфейс прикладного программирования защиты данных (DPAPI) в Windows 2000.
ms.assetid: 048DEA72-39E1-4129-A554-F7D08442C2D9
title: CNG DPAPI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ebd0771b9838b2dbcfbedb3d025a7f650429bba5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127271227"
---
# <a name="cng-dpapi"></a>CNG DPAPI

корпорация майкрософт предоставила интерфейс прикладного программирования защиты данных (DPAPI) в Windows 2000. API состоит из двух функций: [**CryptProtectData**](/windows/desktop/api/dpapi/nf-dpapi-cryptprotectdata) и [**CryptUnprotectData**](/windows/desktop/api/dpapi/nf-dpapi-cryptunprotectdata). DPAPI является частью CryptoAPI и предназначен для разработчиков, которым очень мало известно об использовании криптографии. Эти две функции можно использовать для шифрования и расшифровки статических данных на одном компьютере.

Однако для облачных вычислений часто требуется, чтобы содержимое, зашифрованное на одном компьютере, было расшифровано на другом. таким образом, начиная с Windows 8, корпорация майкрософт расширила концепцию использования относительно удобного API для работы с облачными сценариями. Этот новый API, именуемый DPAPI-NG, позволяет безопасно обмениваться секретами (ключами, паролями, материалами ключа) и сообщениями, защищая их с набором участников, которые можно использовать для снятия защиты с них на разных компьютерах после надлежащей проверки подлинности и авторизации. В настоящее время поддерживаются следующие участники:

-   Группа в лесу Active Directory.
-   Учетные данные веб-сайта.

Дополнительные сведения см. в следующих разделах:

-   [Поставщики защиты](protection-providers.md)
-   [Дескрипторы защиты](protection-descriptors.md)
-   [Формат защищенных данных](protected-data-format.md)

DPAPI-NG построен на основе криптографии следующего поколения (CNG) и включает следующие функции:

-   [**нкрипткреатепротектиондескриптор**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptcreateprotectiondescriptor)
-   [**нкриптклосепротектиондескриптор**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptcloseprotectiondescriptor)
-   [**нкриптпротектсекрет**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptprotectsecret)
-   [**нкрипткуерипротектиондескрипторнаме**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptqueryprotectiondescriptorname)
-   [**нкриптрегистерпротектиондескрипторнаме**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptregisterprotectiondescriptorname)
-   [**нкриптстреамклосе**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptstreamclose)
-   [**нкриптстреамопентопротект**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptstreamopentoprotect)
-   [**нкриптстреамопентаунпротект**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptstreamopentounprotect)
-   [**нкриптстреамупдате**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptstreamupdate)
-   [**нкриптунпротектсекрет**](/windows/desktop/api/NCryptprotect/nf-ncryptprotect-ncryptunprotectsecret)

 

 
