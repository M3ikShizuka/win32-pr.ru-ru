---
description: начиная с Windows 7, каскадные меню создаются с помощью записи реестра подкоманд, записи реестра екстендедсубкоммандскэй или интерфейса иексплореркомманд.
title: Создание статических каскадных меню
ms.topic: article
ms.date: 05/31/2018
ms.assetid: E3A6F174-BE53-48EF-AE9B-A3F297E91B95
api_name: ''
api_type: ''
api_location: ''
topic_type:
- kbArticle
ms.openlocfilehash: d812b4d3d2fb0754002cb37d72718e4fe861ce15
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460512"
---
# <a name="creating-static-cascading-menus"></a>Создание статических каскадных меню

в Windows 7 и более поздних версиях реализация каскадного меню поддерживается с помощью параметров реестра. до Windows 7 создание каскадных меню возможно только с помощью реализации интерфейса [**IContextMenu**](/windows/win32/api/shobjidl_core/nn-shobjidl_core-icontextmenu) . в Windows 7 и более поздних версиях следует прибегнуть к решениям на основе кода объектной модели (COM) только в том случае, если статические методы недостаточны.

На следующем снимке экрана приведен пример каскадного меню.

![снимок экрана, демонстрирующий Пример каскадного меню](images/file-assoc/filecascademenu2ndex.png)

в Windows 7 и более поздних версиях существует три способа создания каскадных меню, которые описаны в следующих разделах.

-   [Создание каскадных меню с помощью записи реестра "подкоманды"](how-to--create-cascading-menus-with-the-subcommands-registry-entry.md)
-   [Создание каскадных меню с помощью записи реестра Екстендедсубкоммандскэй](how-to-create-cascading-menus-with-the-extendedsubcommandskey-registry-entry.md)
-   [Создание каскадных меню с помощью интерфейса Иексплореркомманд](how-to-create-cascading-menus-with-the-iexplorercommand-interface.md)

 

 
