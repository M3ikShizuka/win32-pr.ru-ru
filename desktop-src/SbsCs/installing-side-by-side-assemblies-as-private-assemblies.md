---
description: Для установки параллельных сборок в качестве частных сборок можно установить сборку как компонент пакета установщика.
ms.assetid: 1cfd836f-a1b9-4339-8756-5488c88b3c2b
title: Установка параллельных сборок в качестве закрытых сборок
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f7719a9887f9e92d81e2ad65fe2e75424f0b6957
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127271536"
---
# <a name="installing-side-by-side-assemblies-as-private-assemblies"></a>Установка параллельных сборок в качестве закрытых сборок

Для установки [параллельных сборок](about-side-by-side-assemblies-.md) в качестве [частных сборок](/windows/desktop/Msi/private-assemblies)можно установить сборку как компонент пакета установщика. Это может быть тот же пакет установки, который используется для установки или обновления приложения. Windows Для установки сборок требуется установщик версии 2,0 или более поздней. дополнительные сведения см. в разделе [установщик Windows](../msi/windows-installer-portal.md) SDK и разделах раздела [установка сборок Win32](../msi/installation-of-win32-assemblies.md).

В качестве альтернативы можно использовать установщик для копирования закрытой сборки и манифеста в ту же папку, что и исполняемый файл приложения.

 

 
