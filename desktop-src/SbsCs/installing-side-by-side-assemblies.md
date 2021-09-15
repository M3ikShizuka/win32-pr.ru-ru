---
description: Параллельные сборки можно устанавливать как общие сборки или как закрытые сборки. Дополнительные сведения см. в разделе Установка параллельных сборок в качестве частных сборок и установка параллельных сборок в качестве общих сборок.
ms.assetid: 36f271ff-be0c-4162-8e1c-86088ebddbcc
title: Установка параллельных сборок
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3be68580c7f0e3890c2e53b148daec92fbad18ae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127271523"
---
# <a name="installing-side-by-side-assemblies"></a>Установка параллельных сборок

Параллельные сборки можно устанавливать как [Общие сборки](/windows/desktop/Msi/shared-assemblies) или как [закрытые сборки](/windows/desktop/Msi/private-assemblies). Дополнительные сведения см. в разделе [Установка параллельных сборок в качестве частных сборок](installing-side-by-side-assemblies-as-private-assemblies.md) и [Установка параллельных сборок в качестве общих сборок](installing-side-by-side-assemblies-as-shared-assemblies.md).

Обратите внимание на следующее.

-   сборки, установленные в глобальный кэш сборок установкой с использованием [контекста установки](/windows/desktop/Msi/installation-context) "на пользователя", не защищаются с помощью Windows защиты файлов.
-   сборки, которые устанавливаются в глобальный кэш сборок установкой с использованием [контекста установки](/windows/desktop/Msi/installation-context) для компьютера, защищаются с помощью Windows защиты файлов.

 

 
