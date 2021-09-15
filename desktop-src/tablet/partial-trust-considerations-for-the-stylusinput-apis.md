---
description: Общие сведения о проблемах с частичным доверием и интерфейсе прикладного программирования (API) Стилусинпут.
ms.assetid: 32c26632-03f4-4f21-8c67-ebf38b67d251
title: Рекомендации по частичному доверию для API Стилусинпут
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ceda5edfb2e4133bb0fcb3d260ff1e13f9fdb521
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344746"
---
# <a name="partial-trust-considerations-for-the-stylusinput-api"></a>Рекомендации по частичному доверию для API Стилусинпут

Объект [**RealTimeStylus**](realtimestylus-class.md) , принимающий параметр *Handle* , требует разрешений [UIPermissionWindow. аллвиндовс](/dotnet/api/system.security.permissions.uipermissionwindow?view=dotnet-plat-ext-3.1&preserve-view=true) и [SecurityPermissionFlag. UnmanagedCode](/previous-versions/windows/) в дополнение к разрешениям, необходимым конструктору, принимающему параметр *аттачедконтрол* .

Дополнительные сведения о проблемах безопасности и доверия см. в разделе [безопасность и доверие](security-and-trust.md).

 

 
