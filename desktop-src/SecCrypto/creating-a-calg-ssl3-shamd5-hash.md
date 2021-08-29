---
description: Объясняется, как создать КАЛГ \_ SSL3 \_ SHAMD5 hash.
ms.assetid: dad6fc7f-8abd-4f90-b3e4-8d0169e95087
title: Создание CALG_SSL3_SHAMD5ного хэша
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 567d7fa640c836790265214a7ae99e0ce1a70d925dd0d6c05b3deb1f6bcc81ea
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876670"
---
# <a name="creating-a-calg_ssl3_shamd5-hash"></a>Создание КАЛГ \_ SSL3 \_ SHAMD5 hash

**Создание КАЛГ \_ SSL3 \_ SHAMD5 hash**

1.  Используя стандартную методологию CryptoAPI, создайте MD5 и хэш [*SHA*](../secgloss/s-gly.md) [](../secgloss/h-gly.md) для целевых данных.
2.  Объедините два хэша со значением MD5, крайним левым и самым правым SHA. Это приводит к 36-байтному значению (16 байт + 20 байт).
3.  Получите маркер для [*объекта хэша*](../secgloss/h-gly.md) , вызвав [**CryptCreateHash**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptcreatehash) с калг \_ SSL3 \_ SHAMD5, переданным в параметр *алгид* .
4.  Задайте хэш-значение с помощью вызова [**криптсесашпарам**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptsethashparam). Объединенные хэш-значения передаются в виде **байта** \* в параметре *PBDATA* , и \_ значение HP хашвал должно быть передано в параметр *двпарам* . Вызов [**CryptHashData**](/windows/desktop/api/Wincrypt/nf-wincrypt-crypthashdata) с помощью маркера, возвращенного [**CryptCreateHash**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptcreatehash) на шаге 3, завершится ошибкой.
5.  Вызовите [**криптсигнхаш**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptsignhasha) , чтобы создать сигнатуру.
6.  Вызовите [**криптдестройхаш**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptdestroyhash) , чтобы уничтожить хэш-объект.

 

 
