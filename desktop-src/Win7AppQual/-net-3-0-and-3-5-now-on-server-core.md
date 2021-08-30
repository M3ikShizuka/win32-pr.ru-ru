---
description: .NET 3,0 и 3,5 теперь в Server Core
ms.assetid: 61d6ee20-1304-4a89-b721-4d10a66e47fc
title: .NET 3,0 и 3,5 теперь в Server Core
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d1e81d91e413bc4864f43d3f47f82a9eda42acf9e1ebbc98896eb573554628e8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119999124"
---
# <a name="net-30-and-35-now-on-server-core"></a>.NET 3,0 и 3,5 теперь в Server Core

## <a name="platform"></a>Платформа

**серверы** — Windows Server 2008 R2  



## <a name="feature-impact"></a>Воздействие на функции

 **Серьезность** — низкая  
**Частота** -низкая  





## <a name="description"></a>Описание

вариант установки server Core для Windows server 2008 R2 теперь включает подмножество платформа .NET Framework 3,0 и 3,5, в частности WCF, WF, LINQ.

в варианте установки server Core для Windows server 2008 не поддерживалась поддержка .net.

## <a name="manifestation-of-impact"></a>Влияние на манифесты

это позволяет использовать некоторые приложения на основе WCF и WF, а также приложения, использующие LINQ для выполнения в server Core в Windows server 2008 R2.

## <a name="testing"></a>Тестирование

Протестируйте приложения, включающие WCF, WF и код LINQ в Server Core.

## <a name="links-to-other-resources"></a>Ссылки на другие ресурсы

-   [Server Core](/previous-versions/windows/desktop/legacy/ms723891(v=vs.85))
-   *см. также* разделы "server Core" из пошаговых *руководств по Windows server 2008 R2* , когда они станут доступны.
-   *см. также* раздел «Server Core» *пакета SDK Windows server 2008 R2* , когда он станет доступным

> [!Note]  
> Эти ресурсы могут быть недоступны в некоторых языках и странах или регионах.

 

 

 
