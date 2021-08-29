---
title: Новые в SNMP
description: протокол SNMP поддерживает использование IPv6, начиная с Windows Vista.
ms.assetid: 38d71c0a-8de1-45a7-958c-aa44411451bc
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f0201be821476622c071ba5b92f0c4c6efcb138f7b09e1fc1716e0e51ae6dd87
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119009282"
---
# <a name="new-in-snmp"></a>Новые в SNMP

\[Протокол SNMP доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. вместо этого используйте [служба удаленного управления Windows](/windows/desktop/WinRM/portal), который является реализацией Microsoft WS-Man.\]

протокол SNMP поддерживает использование IPv6, начиная с Windows Vista. однако протокол SNMP поддерживает IPv6 только для сетей, использующих Windows Server 2008 и Windows Vista. Это связано с тем, что для поддержки IPv6 протоколу SNMP требуется обновленный стек протокола, доступный в этих операционных системах.

если сеть не является исключительно сетью Windows Server 2008, связь ipv6 завершится сбоем, даже если на тех компьютерах, где работают предыдущие версии Windows, установлен стек протокола ipv6. например, агенты SNMP, работающие на Windows Server 2003 или Windows XP или Windows 2000, отвечают только на запросы, которые выполняются с их IPv4-адресами.

 

 