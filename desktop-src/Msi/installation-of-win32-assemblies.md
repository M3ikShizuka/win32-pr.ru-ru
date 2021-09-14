---
description: установите сборки Win32, сделав их компонентом пакета Microsoft установщик Windows, который устанавливает или обновляет приложение.
ms.assetid: 09aecb55-ed45-45b3-b27a-d0946223392a
title: Установка сборок Win32
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c9d47847c0c69185a28fa41bbe5c5a05deec1e66
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171780"
---
# <a name="installation-of-win32-assemblies"></a>Установка сборок Win32

установите сборки Win32, сделав их компонентом пакета Microsoft установщик Windows, который устанавливает или обновляет приложение. При создании [таблицы мсиассембли](msiassembly-table.md) и [таблицы мсиассемблинаме](msiassemblyname-table.md)он определяет компонент в \_ столбце Component как сборку. Установщик задаст свойству [**MsiWin32AssemblySupport**](msiwin32assemblysupport.md) версию файла Sxs.dll в операционных системах, которые могут поддерживать сборки Win32, и не задавать это свойство в противном случае.

в Windows Vista и Windows XP установщик Windows не записывает сведения о сборке в реестр. Кроме того, можно использовать общие сборки, закрытые сборки и параллельные сборки. Дополнительные сведения см. в разделе [Общие сборки](shared-assemblies.md), [закрытые сборки](private-assemblies.md)и [Параллельные сборки](side-by-side-assemblies.md).

в следующих разделах описано, как создать пакет установщик Windows для установки сборок Win32 как общего, частного или параллельного использования в разных операционных системах Windows.

-   [установка сборок Win32 для параллельного совместного использования в Windows XP](installing-win32-assemblies-for-side-by-side-sharing-on-windows-xp.md)
-   [установка сборок Win32 для частного использования приложения в Windows XP](installing-win32-assemblies-for-the-private-use-of-an-application-on-windows-xp.md)

 

 



