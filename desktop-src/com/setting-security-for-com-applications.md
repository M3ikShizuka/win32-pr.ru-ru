---
title: Настройка безопасности для приложений COM
description: Настройка безопасности для приложений COM
ms.assetid: 5b615007-e04b-41be-872c-20e0ea818ff1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5a8dd705015aaa2ca1965d07c556ff3d55aada00
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145754"
---
# <a name="setting-security-for-com-applications"></a>Настройка безопасности для приложений COM

Существует несколько способов помочь в управлении безопасностью приложений. Можно изменить параметры безопасности компьютера по умолчанию, используемые всеми приложениями на компьютере, которые не предоставляют собственные значения безопасности. Для конкретного процесса можно настроить безопасность с помощью Dcomcnfg.exe или путем вызова [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity). Можно также программно управлять параметрами безопасности на уровне прокси интерфейса.

В следующих разделах приводятся процедуры, объясняющие, как настроить безопасность:

-   [Изменение параметров безопасности компьютера по умолчанию](modifying-the-security-defaults-for-a-computer.md)
-   [Настройка безопасности Process-Wide](setting-processwide-security.md)
-   [Настройка безопасности на уровне прокси-сервера интерфейса](setting-security-at-the-interface-proxy-level.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Безопасность в COM](security-in-com.md)
</dt> </dl>

 

 




