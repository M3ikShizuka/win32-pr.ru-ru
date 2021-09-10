---
title: Настройка безопасности для приложений COM
description: Настройка безопасности для приложений COM
ms.assetid: 5b615007-e04b-41be-872c-20e0ea818ff1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5a8dd705015aaa2ca1965d07c556ff3d55aada00
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369613"
---
# <a name="setting-security-for-com-applications"></a>Настройка безопасности для приложений COM

Существует несколько способов помочь в управлении безопасностью приложений. Можно изменить параметры безопасности компьютера по умолчанию, используемые всеми приложениями на компьютере, которые не предоставляют собственные значения безопасности. Для конкретного процесса можно настроить безопасность с помощью Dcomcnfg.exe или путем вызова [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity). Можно также программно управлять параметрами безопасности на уровне прокси интерфейса.

В следующих разделах приводятся процедуры, объясняющие, как настроить безопасность:

-   [Изменение параметров безопасности компьютера по умолчанию](modifying-the-security-defaults-for-a-computer.md)
-   [Настройка безопасности Process-Wide](setting-processwide-security.md)
-   [Настройка безопасности на уровне прокси-сервера интерфейса](setting-security-at-the-interface-proxy-level.md)

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Безопасность в COM](security-in-com.md)
</dt> </dl>

 

 




