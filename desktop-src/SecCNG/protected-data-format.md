---
description: Защищенные данные хранятся в виде большого двоичного объекта в кодировке ASN. 1.
ms.assetid: 8E287A1F-4EDF-4068-85F7-59A1D73F7BCD
title: Формат защищенных данных
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3bafa230efd704536e9e30b946e5fbf2d403e664
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067118"
---
# <a name="protected-data-format"></a>Формат защищенных данных

Защищенные данные хранятся в виде большого двоичного объекта в кодировке ASN. 1. Данные форматируются как CMS (синтаксис сообщений сертификата) в виде упакованного содержимого. Цифровой конверт содержит зашифрованное содержимое, сведения о получателе, содержащие зашифрованный ключ шифрования содержимого (CEK), и заголовок, содержащий сведения о содержимом, включая строку правила незашифрованного дескриптора защиты. Это показано на следующей схеме.

![защищенные запечатанные данные](images/protecteddatablob.png)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[CNG DPAPI](cng-dpapi.md)
</dt> <dt>

[Дескрипторы защиты](protection-descriptors.md)
</dt> <dt>

[Поставщики защиты](protection-providers.md)
</dt> </dl>

 

 



