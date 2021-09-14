---
description: Система использует сведения о конфигурации для определения способа запуска службы.
ms.assetid: fc8c631e-076c-4745-8db0-90f46a202e6a
title: Конфигурация службы
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5019469e17fdd0807aa101c7d1e4d6f6019da783
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168896"
---
# <a name="service-configuration"></a>Конфигурация службы

Система использует сведения о конфигурации для определения способа запуска службы. Сведения о конфигурации также включают отображаемое имя службы и ее описание. Например, для службы DHCP можно использовать отображаемое имя "Служба протокола настройки динамического узла" и описание "предоставляет адреса Интернета для компьютера в сети".

Чтобы изменить сведения о конфигурации для объекта службы, программа настройки использует функцию [**чанжесервицеконфиг**](/windows/desktop/api/Winsvc/nf-winsvc-changeserviceconfiga) или [**ChangeServiceConfig2**](/windows/desktop/api/Winsvc/nf-winsvc-changeserviceconfig2a) . Пример см. в разделе [изменение конфигурации службы](changing-a-service-configuration.md).

Чтобы получить сведения о конфигурации для объекта службы, программа настройки использует функцию [**куерисервицеконфиг**](/windows/desktop/api/Winsvc/nf-winsvc-queryserviceconfiga) или [**QueryServiceConfig2**](/windows/desktop/api/Winsvc/nf-winsvc-queryserviceconfig2a) . Пример см. в разделе [запросы к конфигурации службы](querying-a-service-s-configuration.md).

Функции конфигурации службы [**ChangeServiceConfig2**](/windows/desktop/api/Winsvc/nf-winsvc-changeserviceconfig2a) и [**QueryServiceConfig2**](/windows/desktop/api/Winsvc/nf-winsvc-queryserviceconfig2a) поддерживают использование триггеров для управления запуском службы.

Чтобы изменить дескриптор безопасности для объекта SCManager или объекта службы, программа настройки использует функцию [**сетсервицеобжектсекурити**](/windows/desktop/api/winsvc/nf-winsvc-setserviceobjectsecurity) . Чтобы получить копию дескриптора безопасности, программа настройки использует функцию [**куерисервицеобжектсекурити**](/windows/desktop/api/winsvc/nf-winsvc-queryserviceobjectsecurity) .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Настройка службы с помощью SC](configuring-a-service-using-sc.md)
</dt> </dl>

 

 
