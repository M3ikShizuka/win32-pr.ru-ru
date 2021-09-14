---
description: Потоки скриптов ASF в DirectShow
ms.assetid: afef1b8b-4be2-48a1-b72a-b2e6342a5e84
title: Потоки скриптов ASF в DirectShow
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: da279c654a581bdb9eba23371882c5cbefbf5849
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162263"
---
# <a name="asf-script-streams-in-directshow"></a>Потоки скриптов ASF в DirectShow

Когда фильтру [чтения WM ASF](wm-asf-reader-filter.md) присваивается файл, содержащий поток типа вммедиатипе \_ script, он создает для него закрепление вывода, которое можно подключить к фильтру модуля подготовки к [просмотру команды скрипта](internal-script-command-renderer-filter.md) . При вызове [**играфбуилдер:: renderFile**](/windows/desktop/api/Strmif/nf-strmif-igraphbuilder-renderfile)этот фильтр автоматически добавляется в граф и подключается к нему. Когда модуль подготовки отчетов команды скрипта получает пример, содержащий команду сценария, он запускает событие [**события EC \_ OLE \_**](ec-ole-event.md) *, которое содержит скрипт* . Приложение полностью отвечает за обработку этого события.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Чтение файлов ASF в DirectShow](reading-asf-files-in-directshow.md)
</dt> </dl>

 

 



